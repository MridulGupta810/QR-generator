# QR Code Generator

> A sleek, minimal Node.js CLI tool that turns any URL into a scannable QR code — instantly.

---

## What is this?

This is a lightweight command-line application built with **Node.js** that lets you generate QR codes from any URL you provide. It uses the power of:

- **[Inquirer](https://www.npmjs.com/package/inquirer)** — for an interactive, user-friendly CLI prompt
- **[qr-image](https://www.npmjs.com/package/qr-image)** — to generate clean, scalable QR code images
- **Node.js `fs` module** — to save your URL for future reference

No web interface. No bloated dependencies. Just open your terminal, type a URL, and get a QR code.

---

## Preview

When you run the app, you'll be prompted to enter a URL. The tool then generates a `qr_img.png` file and saves the URL to `URL.txt`.

```
? Type in your URL:  https://google.com
The file has been saved!
```

![QR Code Example](qr_img.png)

---

## Features

- Interactive CLI prompt for seamless user experience
- Generates high-quality PNG QR codes
- Automatically saves the entered URL to a text file
- Zero-config setup — just install and run
- Built with modern ES Modules (`"type": "module"`)

---

## Prerequisites

Make sure you have the following installed:

- [Node.js](https://nodejs.org/) (v18 or higher recommended)
- npm (comes bundled with Node.js)

---

## Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/mridulgupta-techie/QR-code-generator.git
   cd QR-code-generator
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

---

## How to Use

### Generate a QR Code

Run the application using Node.js:

```bash
node index.js
```

You'll be prompted to enter a URL:

```
? Type in your URL:  https://your-url-here.com
```

Hit **Enter**, and the tool will:

1. Generate a QR code image → `qr_img.png`
2. Save the URL to a text file → `URL.txt`

### Example

```bash
$ node index.js
? Type in your URL:  https://github.com
The file has been saved!
```

Now open `qr_img.png` — scan it with your phone, and you're good to go!

---

## Project Structure

```
QR-code-generator/
├── index.js          # Main application entry point
├── solution.js       # Reference solution with inline comments
├── package.json      # Project metadata and dependencies
├── package-lock.json # Locked dependency versions
├── qr_img.png        # Generated QR code (created after running)
└── URL.txt           # Saved URL (created after running)
```

---

## Dependencies

| Package    | Version | Purpose                          |
|------------|---------|----------------------------------|
| inquirer   | ^9.3.8  | Interactive CLI prompts          |
| qr-image   | ^3.2.0  | QR code image generation         |
| fs         | ^0.0.1  | File system operations (built-in)|

---

## Tech Stack

- **Runtime:** Node.js
- **Language:** JavaScript (ES Modules)
- **CLI Framework:** Inquirer.js
- **QR Engine:** qr-image

---

## Roadmap

- [ ] Add support for custom QR code sizes
- [ ] Add color customization for QR codes
- [ ] Export QR codes in SVG format
- [ ] Batch URL processing from a file
- [ ] Add a web-based GUI version

---

## Contributing

Contributions are welcome! If you have ideas for improvements or find a bug:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## License

This project is licensed under the **ISC License**.

---

## Acknowledgments

- Built as a learning project to explore Node.js CLI development
- Inspired by the simplicity of modern developer tools

---

<p align="center">
  Made with ❤️ by <a href="https://github.com/MridulGupta810">Mridul Gupta</a>
</p>


