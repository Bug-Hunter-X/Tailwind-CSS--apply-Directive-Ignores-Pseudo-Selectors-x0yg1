# Tailwind CSS @apply Directive Ignores Pseudo-Selectors

This repository demonstrates a bug where Tailwind's `@apply` directive fails to apply styles defined for pseudo-selectors (e.g., `:hover`, `:focus`).  The issue arises because `@apply` only applies the base styles of a class, neglecting styles specific to pseudo-selectors.

**To Reproduce:**
1. Clone this repository.
2. Open `bug.css` and `bugSolution.css`. Observe the difference in behavior.

**Solution:** Avoid using `@apply` with classes containing pseudo-selectors. Direct style application or creating separate classes for base styles and pseudo-selector styles is recommended. 