# css-login-signup — emphasizes it's pure CSS
A responsive Login/Signup form built with pure HTML & CSS — glassmorphism design, animated background, tab switching (no JS), and CSS-only form validation.
# CSS Login/Signup Form

A responsive Login/Signup form built with **pure HTML & CSS** — no JavaScript.

Features glassmorphism design, a colorful animated background, tab switching between Login and Signup (using the checkbox/radio hack), and CSS-only form validation.

## Features

- 🎨 Glassmorphism UI with a frosted, transparent card
- 🌈 Colorful animated background (shifting gradient, floating blobs, rising particles)
- 🔄 Login/Signup tab switching — no JavaScript, just radio inputs + CSS
- ✅ Form validation using native HTML5 attributes (`required`, `pattern`, `minlength`) styled with `:valid` / `:invalid`
- ✨ Smooth animations: card entrance, spinning rainbow border glow, animated gradient text and buttons
- 📱 Fully responsive

## Tech Stack

- HTML5
- CSS3 (Flexbox, custom properties, keyframe animations, `:has()`)

## How to Run

1. Clone this repository
   ```bash
   git clone https://github.com/your-username/css-login-signup.git
   ```
2. Open `login-signup-css-only.html` in your browser — that's it, no build step or dependencies required.

## Validation Notes

Validation is handled entirely by native HTML5 constraints and CSS pseudo-classes (no JS):

- Email fields use `type="email"` for format checking
- Password fields use `minlength` and `pattern`
- Fields turn red/green via `:not(:placeholder-shown):invalid` / `:valid` once the user starts typing
- A checkmark appears on valid fields using the `:has()` selector

**Limitation:** Matching "confirm password" against "password" isn't possible in pure CSS since there's no selector to compare two separate input values — that one check would require a small amount of JavaScript if needed.

## Browser Support

Most features work in all modern browsers. The checkmark animation uses `:has()`, which requires:
- Chrome 105+
- Safari 15.4+
- Firefox 121+

## License

Free to use for learning and personal projects.