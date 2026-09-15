Check Time

World Clock & Time Zone Tracker

Check Time is a lightweight, browser-based world clock and time-zone tracker. It provides a continuously updating clock, date, UTC offset, daylight-saving-time status, Unix epoch time, and convenient time-zone controls in a clean interface.

🌐 Live Demo

Open Check Time

✨ Features

Live clock — Updates automatically every second.

World time zones — Select from the time zones supported by the browser's Intl API.

Automatic local timezone — Starts with the browser's detected timezone.

Date display — Shows the weekday, month, day, and year for the selected timezone.

UTC offset — Displays the current UTC/GMT offset.

DST status — Indicates whether daylight saving time is detected for the selected timezone.

12/24-hour format — Toggle between 12-hour AM/PM and 24-hour time.

Unix epoch — Displays the current Unix timestamp in seconds.

Fullscreen mode — Expand the clock to fullscreen for a distraction-free display.

Responsive interface — Designed to work across desktop and mobile browsers.

No backend required — Time calculations are performed directly in the browser.

🖥️ Interface

The application includes:

A large live time display.

The current date for the selected timezone.

A timezone selector.

Information cards for:

UTC Offset

DST

Time Format

Unix Epoch

Controls for time-format switching and fullscreen mode.

🛠️ Technology

Check Time is intentionally simple and dependency-free:

HTML5 — Page structure

CSS3 — Styling and responsive layout

Vanilla JavaScript — Application logic

ECMAScript Internationalization API (Intl) — Timezone-aware date/time formatting

Fullscreen API — Fullscreen functionality

GitHub Pages — Static hosting

The repository currently consists of a single index.html application file and a LICENSE file. The implementation uses the browser's Intl.DateTimeFormat and Intl.supportedValuesOf('timeZone') APIs where available.

🚀 Run Locally

No build system or package installation is required.

Option 1 — Open directly

Clone the repository:

git clone https://github.com/wfkm01-eng/Check-Time.git
cd Check-Time

Then open index.html in a modern web browser.

Option 2 — Use a local web server

For a more production-like environment, serve the directory with a local HTTP server.

Using Python:

python -m http.server 8000

Then open:

http://localhost:8000

📁 Project Structure

Check-Time/
├── index.html
├── LICENSE
└── README.md

⚙️ How It Works

When the page loads, the application:

Detects the browser's current timezone.

Builds the timezone selector using Intl.supportedValuesOf('timeZone') when supported.

Falls back to a predefined list of common timezones in browsers without that API.

Formats the current time using Intl.DateTimeFormat.

Calculates the selected timezone's UTC offset.

Checks DST status by comparing January and July offsets.

Calculates the Unix epoch timestamp.

Refreshes the displayed values every second.

Changing the timezone immediately refreshes the displayed information. The 12/24-hour control changes the presentation without requiring a page reload.

🌍 Browser Compatibility

A modern browser with support for the JavaScript Internationalization APIs is recommended.

The application is designed to work with current versions of:

Google Chrome

Microsoft Edge

Mozilla Firefox

Safari

Other modern browsers with Intl.DateTimeFormat support

Intl.supportedValuesOf('timeZone') is used when available, with a fallback timezone list for browsers that do not provide it.

🔒 Privacy

Check Time does not require an account, server-side database, or application-specific backend.

The selected timezone and clock calculations are handled in the browser. The application does not need to send your clock information to a remote service.

📜 License

This project is distributed under the GNU General Public License v3.0 (GPL-3.0). See the LICENSE file for the complete license text.

👤 Author

Created by wfkm01-eng.

GitHub: https://github.com/wfkm01-eng

Repository: https://github.com/wfkm01-eng/Check-Time

Live Demo: https://wfkm01-eng.github.io/Check-Time/

❤️ Credits

Check Time — World clock & Time Zone Tracker

Built with ❤️ using HTML, CSS, and JavaScript.
