# Project memory

## Product intent & audience

- Personal portfolio for Hemanth: bio, app logo, banner image, and BackOffice AI business management platform details.
- Includes an interactive AI assistant feature with answer logic.
- Supports user accounts (username/password) with persistent saved data.

## Brand personality & voice

- Professional, personal-portfolio tone introducing Hemanth and his BackOffice AI product.

## Visual design & UX direction

- Stack: Vite + React (JSX), Tailwind CSS, React hooks, Lucide React icons.
- Import project modules via `@/` path alias (maps to `src/`).
- App runs in a preview environment; users refresh/reopen preview after fixes.

## Decisions, constraints & rationale

- Avoid installing extra UI/theme/icon packages beyond the default template stack.
- User data persists across sessions; login required to access saved data after reload.
- A prior runtime crash was caused by a duplicate variable name in the AI assistant answer logic — now fixed and build verified clean.

## Open questions & assumptions

- "Single-file web application" in the summary may conflict with the `@/` path alias / `src/` structure; current code likely uses modular files under `src/`.
- Scope of the AI assistant (content topics, auth gating, data storage mechanism) is not fully specified.