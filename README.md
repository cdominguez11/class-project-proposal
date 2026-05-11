# LockedIn

A minimal, distraction-free focus timer with a built-in task list — built for CPSC 20000 at Lewis University.

**Live app:** https://cdominguez11.github.io/class-project-proposal/LockedIn.html
**Proposal:** [index.html](index.html)

---

## What Was Delivered

All features from the [Class Project Proposal](index.html) were implemented:

### Standard Features (Requirement 2)
| Feature | Description |
|---|---|
| Editable countdown timer | Click the time display to set any duration; supports h:mm:ss and mm:ss formats |
| Task list | Add, complete, and delete tasks; completed tasks move to the bottom with strikethrough |
| Light / dark mode | Automatically follows the operating system setting via CSS `prefers-color-scheme` |
| Keyboard shortcuts | `Enter` starts, `Space` pauses, `Escape` cancels edit, `?` opens help |
| Session complete notification | In-app banner slides in; browser notification fires if permission is granted |

### Advanced Features (Requirement 3)
| Feature | Description |
|---|---|
| Accurate background timing | Uses `Date.now()` to compute elapsed real time so the timer stays correct even when the browser tab is hidden or throttled |
| `contentEditable` inline editing | Tasks are edited directly in place — no separate input box; `Backspace` on an empty task deletes it |
| CSS animations | Timer pulses when under 60 seconds, flashes when done; tasks fade in on add |
| Web Notifications API | Requests permission on load and fires a native OS notification when the session ends |
| Keyboard shortcut system | Context-aware — shortcuts are suppressed while typing in the timer or task input so nothing breaks |

---

## How to Use

Open `LockedIn.html` in any modern browser, or visit the live link above.

- **Set your time** — click the large timer and type a duration (e.g. `2500` becomes `25:00`)
- **Start** — press `Enter` or click the timer and hit Enter
- **Pause / Resume** — press `Space`
- **Add tasks** — type in the bottom-left field and press `Enter`
- **Complete a task** — click the `–` bullet next to it
- **Delete a task** — click the `×` bullet on a completed task
- **Help** — press `?` anytime for the full controls reference

---

## Technology

- HTML, CSS, JavaScript — no frameworks, no build step, runs as a single file
- [Bebas Neue](https://fonts.google.com/specimen/Bebas+Neue) + [DM Mono](https://fonts.google.com/specimen/DM+Mono) via Google Fonts
- Web Notifications API
- CSS Grid layout

---

## Acknowledgments

Thank you to Professor Eric Pogue for an excellent semester — the foundations you taught in this course made every part of this project possible.

This project was also completed with the assistance of [Claude Code](https://claude.ai/code) by Anthropic, which helped accelerate development and polish the final product.

---

*MIT License — Christopher Dominguez Ramirez, 2026*
