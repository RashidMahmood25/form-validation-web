# Form Validation Demo — Sign-Up Form (Web)

A single-page registration form with live JavaScript validation.
Errors appear as you type, fields turn green/red, and the submit button stays
disabled until every field is valid.

## What is validated

- **First / last name** — required, at least 2 letters, letters/spaces only
- **Email** — required, standard `name@domain.tld` format
- **Mobile (Pakistan)** — required, 11 digits starting with `03` (e.g. 0301-2345678)
- **Date of birth** — required, must be a real past date, age 13 or older
- **City** — optional dropdown (Karachi, Lahore, Islamabad, …)
- **Password** — required, 8+ characters with a letter and a number, with a live
  strength meter (length, mixed case, digits, symbols)
- **Confirm password** — must match
- **Terms checkbox** — must be accepted

On success the form shows a confirmation summary — **demo only, nothing is sent
to a server**.

## How to use

1. Open `index.html` in any modern browser (double-click the file, or serve the
   folder with any static server).
2. Fill in the form — validation runs on every keystroke and on blur.
3. Try wrong values on purpose (bad email, short password, mismatched
   confirmation) to see each error message.

No build step, no dependencies, no data leaves your browser.

## What was practiced

- Single self-contained HTML/CSS/JS page
- Live validation with `input` / `blur` / `change` events and regex checks
- Password-strength scoring and a visual meter
- Enabling/disabling submit based on overall form validity
- `novalidate` so the custom JavaScript messages are used instead of the
  browser's built-in ones
