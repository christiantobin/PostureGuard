# 🤝 Contributing to PostureGuard

Thanks for your interest in contributing to **PostureGuard**! This project aims to promote better posture and wellness while working at a computer. Whether you're here to fix a bug, add features, or improve posture detection — you're welcome here.

---

## 🚧 Forking Workflow

To keep the main repository clean, **please do not create branches directly in this repository.**

Follow these steps to contribute:

1. **Fork the repository**  
   Click the "Fork" button at the top right of this page and create your own copy.

2. **Clone your fork**
   ```bash
   git clone https://github.com/your-username/PostureGuard.git
   cd PostureGuard
   ```

3. **Create a feature branch in your fork**
   ```bash
   git checkout -b feature/your-feature-name
   ```

4. **Push to your fork and open a Pull Request**
   ```bash
   git push origin feature/your-feature-name
   ```

5. Open a Pull Request against `master` in the **original** repository (this one).

---

## ✅ Pull Request Expectations

When opening a PR:

- Provide a **clear summary** of what your changes do.
- If it’s a new feature, include brief testing steps.
- If you're changing posture detection behavior, please make it **easily swappable or mockable** (no hardcoded webcam logic unless modular).
- Keep PRs **small and focused** — avoid mixing unrelated changes.

---

## 📦 Code Guidelines

We’re keeping this project flexible and approachable. Please:

- Use **descriptive function and variable names**.
- Leave **comments** for non-obvious logic (especially around posture simulation or UI focus tricks).
- Prefer **cross-platform** solutions where possible (Windows, Linux, macOS).
- Avoid using obscure dependencies unless truly necessary.

---

## 🧪 Testing Tips

If your work changes behavior:

- Test posture lock and unlock flows.
- Simulate posture correction and verify the white screen dismisses.
- Make sure the override key (e.g., Ctrl+Q) still works.
- Confirm the app auto-dismisses after the timeout period.

---

## 🧠 For New Contributors

You can get started with these files:

- `PROJECT_GUIDE.md` — high-level user stories and scope.
- `README.md` — setup and running instructions.
- Code is organized to separate posture logic and screen control.

If you're not sure where to start, open an issue or ask for help in your PR.

---

Thanks for helping improve PostureGuard 🙌
