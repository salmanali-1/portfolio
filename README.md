# Salman Ali: Personal Portfolio Website

**Assignment #2: Design a Three-Page Website Using HTML and CSS** (Web Technologies, BSCS Semester 5)

- **Name:** Salman Ali
- **Roll number:** FA24/BSCS/392
- **Section:** I
- **University:** Lahore Garrison University
- **Topic chosen:** Personal Portfolio
- **GitHub repository:** _add your repository URL here_
- **Live website:** _add your GitHub Pages URL here_

## Pages and CSS methods

| File | Purpose | CSS method |
| --- | --- | --- |
| `index.html` | Home: introduction, experience, skills | Inline CSS (style attributes) |
| `information.html` | Projects and services: article, aside, table, audio, video | Embedded CSS (style element) |
| `registration.html` | Project inquiry form | External CSS (`style.css`) |

Media files: `images/brake-disc.svg`, `media/welcome-chime.mp3`, `media/brake-disc-preview.mp4`.

## Validation

All three pages were checked with the Nu HTML Checker, the engine behind the W3C Markup Validation Service, with no errors reported. Screenshots from https://validator.w3.org/ go in the `screenshots/` folder:

- `screenshots/index-validation.png`
- `screenshots/information-validation.png`
- `screenshots/registration-validation.png`

## Browser testing

| Test | Expected result | Chrome | Firefox |
| --- | --- | --- | --- |
| Submit with empty required fields | Browser blocks submission and highlights the first empty field | | |
| Enter an invalid email | Browser asks for a valid email address | | |
| Enter a password shorter than 8 characters | Browser reports the minimum length | | |
| Enter an age below 18 or above 99 | Browser reports the allowed range | | |
| Type more than 500 characters in comments | Typing stops at 500 characters | | |
| Hover and focus styles | Buttons and links change colour; inputs show a green outline | | |
| Audio and video playback | Both clips play with controls | | |

Differences noted: _write any differences you saw between the two browsers here (for example, the look of the date picker or the wording of validation messages)._

## Short Explanation

CSS (Cascading Style Sheets) is the language that controls how HTML content looks: colours, fonts, spacing and layout. Its main benefits are separating content from presentation, keeping a consistent design across pages, reducing repeated code and making a site easier to maintain.

A CSS rule has a selector, a property and a value. In information.html the rule `.notice { background-color: #f3e3d6; }` uses the class selector `.notice`, the property `background-color` and the value `#f3e3d6`, giving the announcement box a soft terracotta background.

Inline CSS is written in a style attribute on a single element, as on index.html. It is quick but hard to reuse. Embedded CSS sits in a style element in the page head, as on information.html; it styles one whole page but cannot be shared. External CSS lives in a separate file linked with a link element, as style.css is on registration.html; one file can style many pages and browsers can cache it, so it suits real projects best.

CSS1 (1996) introduced basic font, colour and text styling. CSS2 (1998) and CSS2.1 added positioning, media types and table styling, and CSS2.1 corrected errors to become a stable baseline. Modern CSS is split into independent modules, such as Selectors, Flexbox, Grid and Media Queries, which are developed separately, so new features arrive faster.

Browser support matters because browsers can interpret HTML and CSS slightly differently, so a feature may look different or fail in one of them. I tested the site in Google Chrome and Mozilla Firefox, checking layout, media playback and form validation.

Semantic HTML describes meaning: for example, the nav element holding the main links on every page. Non-semantic HTML has no meaning of its own: for example, the span with class hint that holds the helper text under form fields in registration.html.
