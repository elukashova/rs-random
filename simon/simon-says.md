# Simon Says

## Task

### Description

The task is a variant of the classical [Simon Says](https://en.wikipedia.org/wiki/Simon_says) game, where players must remember and reproduce sequences of keyboard symbols.

### Task objective

To practice event handling, such as clicks and keyboard inputs.

### Game rules

- The game consists of **15 levels**.
- Each level represents a round where the user must repeat **a sequence of keyboard symbols**.
- The first round starts with **2 symbols**.
- Each new round increases the sequence length by **one symbol**.
- **A rounds counter** displays the current level.
- The user can use both **virtual** _(by clicking letter keys on the screen)_ and **physical** keyboards _(by pressing letter keys on their keyboard)_ to play the game.

- The initial game screen displays a virtual keyboard and the "Start" button.
- To start the first level, the user clicks the “Start” button. 
- When the first round begins, the “Start” button is replaced by the “Repeat the sequence” button.
- Only after clicking the “Start” button is the first sequence shown by simulating the typing of the corresponding symbols on the virtual keyboard. The typing simulation should be clear: the symbols are “typed” one after another, and the corresponding keys are highlighted.
- The “Repeat the sequence” button is disabled while the current sequence is being reproduced.
- The user can click the “Repeat the Sequence” button **only once**. After that, the “Repeat the sequence” button is replaced by the “Start over” button.
- When answering by clicking the keys on the virtual keyboard, these keys should be highlighted upon clicking.
- When answering by pressing keys on the physical keyboard, the corresponding keys on the virtual keyboard should be highlighted upon pressing.
- The user is allowed only **one incorrect answer per round**. After a second incorrect attempt, the “Repeat the sequence” button, if still present, is replaced by the “Start over” button.
- The user can click the “Start over” button to restart the game from the first round. In this case, the “Start over” button is replaced by the “Start” button, and the rounds counter is reset accordingly.
- Feedback is provided after an incorrect answer. This can be implemented by displaying a message, a sound, or a visual cue.
- When the user answers correctly, the “Repeat the sequence” button (or, if already clicked, the “Start over” button) is replaced by the “Next” button.
- Feedback is provided after a correct answer. This can be implemented by displaying a message, a sound, or a visual cue.
- After clicking the “Next” button, the new level starts by reproducing the next sequence, and the rounds counter is updated accordingly.
- Upon successfully completing the 15th round, feedback is provided (through a message, sound, or visual cue) to indicate that the game is over, and the “Repeat the sequence” button (or, if already clicked, the “Start over” button) is replaced by the “Play again” button.
- After clicking the “Play Again” button, the game restarts from the first round, and the rounds counter is reset.

### Main functional requirements

- Initially, `body` in the index.html file should be empty (only script tag is allowed).
- All necessary elements are generated using `createElement()` function. No `html` injection is allowed.
- The design should be **adaptive (or responsive)** from _(500px <= width)_.
- The sequence is randomly generated for each new round.
- The design is at your discretion.
- The application should be done **in English**.

## Repository requirements

- The task should be done in private school's repository.
- The code should be committed to a separate branch **named (`simon-says`)**.
- The **main** (or **master**) branch should be empty (contain only files like README.md, .gitignore or .github folder)
- Commits should represent the work history. Commit messages should follow the [guideline](https://www.conventionalcommits.org/en/v1.0.0/)
- Once the work is finished, create a pull request from a development branch to main (or master). This PR doesn't need to be merged.
- The pull request name should contain **the task name**.
- The pull request description should contain the following information:
  - link to the task
  - screenshot of your application (one would be enough)
  - link to your application
  - date of completion/deadline
  - your self-check with a preliminary evaluation that is based on the evaluation criteria from the task
- Submit **a link to deploy** in Cross-Check: Submit tab.

## Technical requirements

- The application is checked in the latest version of Google Chrome browser.
- It is **not allowed** to use:
  - CSS frameworks (e.g., `Bootstrap`),
  - JS frameworks (e.g., `Angular`, `React`, `Vue`, etc.),
  - Outdated libraries (e.g. `JQuery`, etc.),
  - Any JS libraries which are not devDependencies (e.g. `lodash`),
  - `TypeScript`.
- You **can** use bootstrap, CSS frameworks, HTML and CSS preprocessors, and `normalize.css` or `modern-normalize`.
- JS code **must not be minified** to facilitate the cross-check process.
- It is strongly recommended to use `eslint` and `prettier`.

## CrossCheck Criteria 
_It is recommended to print the right answer for each round in the browser's console to facilitate the cross-check process._

## Penalties

## Useful links:

- [DOM](http://learn.javascript.info/document)
- [Event](http://learn.javascript.info/event-details)
- [An Introduction To DOM Events](https://www.smashingmagazine.com/2013/11/an-introduction-to-dom-events/)
- [Keyboard events](https://learn.javascript.info/keyboard-events)