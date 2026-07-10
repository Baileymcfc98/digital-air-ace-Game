# Digital Air Ace

A quick, touchscreen-friendly digital systems and responsible AI quiz game designed for a Further Education induction stall.

Learners answer eight rapid questions. Correct answers destroy a fictional enemy aircraft; incorrect answers cost a life. Where several learners achieve the same number of correct answers, the leaderboard ranks them by their total response time.

## Play locally

Double-click `index.html` and open it in Microsoft Edge or Google Chrome.

## Publish with GitHub Pages

1. Create a new **public** GitHub repository.
2. Extract this ZIP file.
3. Upload `index.html`, `README.md` and `.nojekyll` to the root of the repository.
4. Commit the files.
5. In the repository, open **Settings → Pages**.
6. Under **Build and deployment**, choose **Deploy from a branch**.
7. Select the `main` branch and the `/ (root)` folder.
8. Select **Save**.

GitHub will then provide the public address for the game.

## Recommended stall setup

- Open the GitHub Pages address in Edge or Chrome.
- Use the **Full Screen** button before learners arrive.
- Keep the same browser and device throughout the event.
- Avoid private or incognito browsing.
- Use the in-game **Reset Scores** button when you want to start a fresh leaderboard.

## Leaderboard storage

The leaderboard is saved in the browser's local storage.

It remains after the browser or computer is restarted, but it is specific to that browser and device. Separate stall laptops will therefore have separate leaderboards. Clearing browser data, changing the GitHub Pages address, or using private browsing can remove the stored scores.

## Editing the questions

Open `index.html` in a text editor and search for:

```javascript
const QUESTION_BANK = [
```

Each question contains:

- `category`
- `question`
- four `answers`
- `correct`

The correct-answer numbering begins at zero:

- `correct: 0` — first answer
- `correct: 1` — second answer
- `correct: 2` — third answer
- `correct: 3` — fourth answer

The game randomly selects eight questions for each attempt.

## Notes

- No login or database is required.
- The game can run offline when opened directly from the downloaded HTML file.
- All aircraft, emblems and squadrons are fictional.
- No real-world political symbols are used.
