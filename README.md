# WeekLoad

**See which school days are overloaded, then spread the work out.**

WeekLoad is a free, mobile-friendly web app that adds up the "stress" of every school day, so students and teachers can spot a crushing day *before* it happens.

**Live app:** https://natna31.github.io/weekload/
**Demo video:** https://youtu.be/okILf4LRXfA
**Made for:** CSC Back-to-School Hackathon 2026

---

## The problem

Students often have three tests and two projects due on the same day. Each teacher plans their own schedule, but no teacher can see what the others have already set. The result is stress, rushed work and lower grades.

## The idea

Every deadline adds **stress points** to its date. A day's total decides its color, so an overloaded day is obvious at a glance.

| Deadline type | Points |
|---|---|
| Test | 3 |
| Project | 3 |
| Quiz | 2 |
| Homework | 1 |

| Day total | Level |
|---|---|
| 0 | Free |
| 1-2 | Light |
| 3-4 | Busy |
| 5 or more | Overloaded |

You can change the point values and the overload threshold in Settings.

## Try it in 30 seconds

The app starts **empty** on purpose.

1. Open the live app.
2. Go to **Settings** and tap **Add example deadlines** (or add your own with the **+** button).
3. Go back to **Calendar**. You will see overloaded days in red, with an alert icon and the point total.
4. Tap a red day, tap **Move** on a deadline, and pick a lighter day.
5. Try **Find a lighter day** and **Build my study plan**.

## Features

- **Heatmap calendar** with a 4-week view and Back / Today / Next buttons
- **Add, edit, move and delete** deadlines, with Undo for deletes
- **Move flow:** shows the lightest school days and the before/after load
- **Teacher tool, "Find a lighter day":** suggests the 3 lightest school days for a new test, project or quiz
- **Student tool, "Spread out my studying":** puts study sessions on your lightest days before a deadline
- **This week:** a day-by-day agenda with a "tomorrow" summary
- **Insights:** overloaded days, busiest day, average load per school day, load by week, points by subject, and a tip
- **Settings:** dark mode, adjustable points, copy/paste backup, clear all data
- **Welcome screen** for first-time users (student or teacher view)

## How it works

- Each deadline has a type, and each type has a point value.
- A day's load is the sum of its deadlines' points.
- Calendar colors, lighter-day suggestions and study plans all come from simple sorting by that load.
- **There is no AI inside the app.** It is plain, readable logic, and all of the code is in one file.

## Privacy

- Everything is saved in your browser (`localStorage`) on your own device.
- No accounts, no tracking, no servers, no outside APIs.
- Nothing is sent anywhere. Use **Copy my data** / **Paste data** in Settings to move your deadlines to another device.

## Design and accessibility

- Soft "neumorphism" interface designed in Google Stitch
- Responsive layout: bottom tab bar on phones, side bar on tablets and desktops, and text size that scales with the screen
- Every calendar day shows its **point number as text**, and overloaded days add an alert icon, so the app never relies on color alone
- Large tap targets, visible keyboard focus, pop-ups that trap focus and close with Escape
- Light and dark themes

## Built with

- HTML, CSS and vanilla JavaScript in a single file (`index.html`)
- No frameworks, libraries or build tools
- Hosted on GitHub Pages

## Run it yourself

Download `index.html` and open it in any browser. Nothing to install.

## AI-use disclosure

I used **Claude** to brainstorm the idea, plan the features and help write and test the code, and **Google Stitch** to design the interface. I chose the problem and the points system, tested the app, and can explain how the heatmap, the lighter-day suggestions and the study-plan sorting work.

## How WeekLoad matches the judging criteria

| Criteria | In WeekLoad |
|---|---|
| **Learning** | Simple points logic, one readable file, and an honest AI-use disclosure |
| **Design** | One clear calendar, a simple flow, and a layout that adapts to phones, tablets and desktops |
| **Creativity** | Looks at workload across all classes at once, with tools for both teachers and students |
| **Functionality** | Every feature works: add, edit, move, delete, undo, suggestions, study plans, insights, settings and backup |
| **Impact** | Helps students avoid stacked deadlines and helps teachers pick fairer test days |

## Limitations and what's next

- Data lives on one device and does not sync between devices.
- Suggestions only use school days (Monday to Friday).
- **Next:** an optional shared school calendar, so teachers and students see one combined view, plus reminders and class sharing by code.

## Author

Natnael ([@natna31](https://github.com/natna31))
