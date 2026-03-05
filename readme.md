# Contact Form (Web3Forms API)

A simple responsive contact form built with HTML and CSS, connected to the Web3Forms API for form submission.

## Features

- Clean contact form UI with responsive layout
- Full-screen background image
- Required validation for all form fields
- Direct POST submission to Web3Forms endpoint

## Project Structure

- `index.html` - Form markup and API integration
- `form.css` - Styling and responsive behavior
- `readme.pdf` - Existing document

## Form Fields

The form includes:

- `name` (text, required)
- `email` (email, required)
- `message` (textarea, required)
- `access_key` (hidden field for Web3Forms)

## How It Works

1. User fills out the form in `index.html`.
2. On submit, data is sent using `POST` to:
   - `https://api.web3forms.com/submit`
3. Web3Forms handles delivery based on the configured access key.

## Run Locally

1. Clone or download this project.
2. Open `index.html` in a browser.

No build tools or dependencies are required.

## Important Security Note

The `access_key` is currently hardcoded in `index.html` and exposed on the client side.

For safer production usage:

- Use an environment-based/server-side flow when possible
- Rotate the key if it is public or shared
- Add spam protection (captcha/honeypot/rate limits)

## Customization

- Change headings/labels directly in `index.html`
- Modify colors, spacing, and responsive breakpoints in `form.css`
- Replace the background image URL in `form.css`

## License

This project is for learning/demo purposes.
