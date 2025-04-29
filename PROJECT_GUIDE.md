# 📐 PostureGuard: Project Guide

**PostureGuard** is a wellness-focused desktop application that encourages users to maintain proper posture. When poor posture is detected, the app temporarily takes over the screen with a white overlay to nudge the user to correct their posture. The user can return to normal activity either by fixing their posture or using a manual override key.

---

## 📋 User Stories

### 1. Visual Reminder for Bad Posture
> As a user, I want to be visually interrupted when my posture is poor so that I’m reminded to sit correctly.

- The screen should go white, filling the entire display.
- All user interaction (mouse, keyboard, etc.) should be blocked during this time.
- The mouse cursor should be hidden.

---

### 2. Automatic Dismissal on Good Posture
> As a user, I want the overlay to disappear automatically once I fix my posture so I can continue working naturally.

- Posture should be monitored continuously while the screen is locked.
- As soon as the user sits correctly, the white screen disappears.

---

### 3. Manual Override Key
> As a user, I want to be able to exit the white screen manually using a specific key combination in case I need to regain access.

- The override should be hard to trigger accidentally (e.g., Ctrl+Q).
- The shortcut should immediately remove the overlay.

---

### 4. Safety Timeout
> As a user, I want to know I’ll never be permanently locked out, even if the posture system fails.

- There should be a configurable maximum lockout time (e.g., 30 seconds).
- After this time, the screen unlocks even if posture hasn’t improved.

---

## 🧩 Implementation Tasks

### Core Behavior
- [ ] Build a full-screen white overlay window.
- [ ] Ensure the window cannot be closed or minimized normally.
- [ ] Hide the mouse cursor while the overlay is active.
- [ ] Prevent interaction with other applications while the screen is locked.
- [ ] Allow the overlay to be dismissed by pressing a specific key combination (e.g., Ctrl+Q).
- [ ] Add a safety timeout that automatically dismisses the screen after N seconds.

### Posture Detection (Basic or Simulated)
- [ ] Simulate or detect “bad posture” to trigger the white screen.
  - This could be done with a camera, or simply simulated with a button, timer, or keystroke.
- [ ] Continuously check for improved posture while the overlay is active.
- [ ] Automatically dismiss the screen when posture improves.

### Optional Enhancements
- [ ] Allow configuration of timeout and override key via a file or simple interface.
- [ ] Add a system tray icon or background indicator to show the app is running.
- [ ] Track and log each screen-lock event (e.g., timestamp, duration).
- [ ] Allow future posture detection modules to be plugged in easily.

---

## 🧪 Deliverables

- A working desktop application that demonstrates the core functionality.
- A short guide (`README.md`) explaining how to run and test it.
- A clear placeholder for posture detection logic that can be improved over time.

---

## 💡 Tips for Development

- You may simulate posture correction with a key press or button for testing.
- Focus on user experience: keep the overlay smooth and hard to ignore.
- Prioritize safety and recovery: never permanently lock the user out.

---

Happy building!
