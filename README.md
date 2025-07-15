# File Bundler & Unbundler

- This project provides a web-based utility for bundling and unbundling markdown multi-file code projects using a classic Mac System 7-inspired interface. It enables users to package entire directory structures into a single Markdown file and later extract them back to their original files and folders, all within the browser.
- You can use this to send lots of source code files between Google AI Studio and You
- The Mac System 7 is for fun only


**Technologies Used:**  
- Semantic, standards-compliant HTML5  
- Modern, modular JavaScript (ES6+) for all interactivity and file processing  
- CSS3, including custom fonts and advanced layout, for authentic Mac System 7 theming  
- [JSZip](https://stuk.github.io/jszip/) for client-side ZIP archive creation  
- Web APIs: FileReader, Blob, and directory file input  
- No frameworks or build tools required; fully self-contained and portable
- System7css-master based on [pfcode](https://github.com/pfcode/system7css)

## Features

- **File Bundler:** Select a local directory and bundle all files (with structure) into a single Markdown file using custom delimiters.
- **File Unbundler:** Upload a Markdown bundle and extract all files as a ZIP archive, preserving the original directory structure.
- **Classic UI:** Faithful Mac System 7 look and feel, including menu bar, window chrome, and 3D status bars.
- **Client-Side Only:** No server or backend required; all processing is done in the browser for privacy and speed.

## Markdown Bundling/Unbundling structure

- Each file in the bundle is delimited in the Markdown by a start tag # --- START FILE: <relative/path/to/file.ext> --- and an end tag # --- END FILE: <relative/path/to/file.ext> ---, with the file’s content placed between these tags; each file section is separated by a blank line, and the relative path preserves the original directory structure.

## Installation & Usage

1. **Clone or Download:**
   - Download the repository as a ZIP or clone it using:
     ```
     git clone https://github.com/yourusername/mac-system7-bundler-unbundler.git
     ```
2. **File Structure:**
   - Place all files in a single directory, preserving the folder structure (especially for CSS, fonts, and images).

3. **Run the App:**
   - Open `BundlerUnbundler.html` in any modern web browser (Chrome, Firefox, Edge, Safari).
   - No installation or build step is required.

4. **Bundling Files:**
   - In the "File Bundler" window, select a directory using the provided file input.
   - The app will generate a Markdown bundle containing all files and their relative paths.
   - Download the bundle using the provided button.

5. **Unbundling Files:**
   - In the "File Unbundler" window, upload a previously created Markdown bundle.
   - The app will parse the bundle and allow you to download a ZIP archive with the original files and structure.

## License

MIT

## About

This project uses advanced front-end engineering skills, including DOM manipulation, file handling, and custom UI theming, using only native web technologies.  
If you are a recruiter or hiring manager, you can review the full source code in this repository to evaluate my proficiency in modern HTML, CSS, and JavaScript.

---

## Files to Upload to GitHub

To make your project complete and functional for others, upload the following files and folders:

- `BundlerUnbundler.html` (main app)
- `css/normalize.css` (CSS reset)
- `css/layout.css` (Mac System 7 theme)
- `fonts/` (Chicago and MonoLisa-Regular font files)
- `img/` (Apple icon, window title bar backgrounds, and any other UI images)
- `README.md` (this file)
- `LICENSE` (optional, but recommended; for MIT, you can use [this template](https://opensource.org/license/mit/))

**Folder structure example:**
```
/
├── BundlerUnbundler.html
├── README.md
├── LICENSE
├── css/
│   ├── normalize.css
│   └── layout.css
├── fonts/
│   ├── ChicagoFLF.ttf
├── img/
│   ├── header_apple.png
│   └── window_titlebg.png
```
