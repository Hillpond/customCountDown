# Custom Countdown

A small single-page web application for creating and managing custom countdown timers  
(e.g. exams, deadlines, trips).

Live site: https://hillpond.github.io/customCountDown/

---

## Features

- **Custom countdowns**
  - Provide a name and choose any date and time.
- **Persistent storage**
  - Countdown data is stored in the browser via `localStorage`.
  - Timers remain available across page reloads and browser restarts
    (until site data is cleared).
- **Overview dashboard**
  - Landing page lists all active countdowns.
  - Each card shows a live mini-countdown in days, hours, minutes, and seconds.
- **Detail view**
  - Clicking a card opens a focused “doomsday clock” for that timer.
  - Multiple display modes:
    - Full (days, hours, minutes, seconds)
    - Hours only
    - Minutes only
    - Seconds only
- **Management**
  - Individual countdowns can be deleted from the overview.

---

## Technology

The project is implemented using only **HTML**, **CSS**, and **vanilla JavaScript**.

- No frameworks or build tools are required.
- Time calculations use the built-in `Date` object and `setInterval`.
- Data is stored in `localStorage` under the key:

  ```js
  "doomsdayEvents"
