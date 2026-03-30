# Code Style — Frontend

## JavaScript/React
- React 18, MUI v5
- ESLint + Prettier
- camelCase for variables/functions
- PascalCase for components and files
- Named exports preferred over default exports
- Functional components only (no class components)
- Custom hooks: `useXxx` naming

## MUI conventions
- Use MUI components, not raw HTML where MUI equivalent exists
- Theme tokens for colors/spacing, never hardcoded hex
- `sx` prop for one-off styles, `styled()` for reusable
- Follow FPT Cloud console design system (dark sidebar, white content area)

## File structure per component
```
src/components/FeedbackWidget/
├── index.js          ← entry point, named export
├── FeedbackWidget.jsx ← main component
├── FeedbackWidget.test.jsx
└── hooks/
    └── useFeedback.js
```
