# Change Log

## 2.1.2 (June 1st, 2020)

**Implemented enhancements:**

- Upgrade `use-elapsed-time` package to v2.1.3 which replaces `useLayoutEffect` with `useEffect` when the environment is node for SSR and removes side effects from `useState` so React.StrictMode works as expected in development

## 2.1.1 (May 21st, 2020)

**Big fix:**

- Fix an issue where rounding numbers with bitwise shifting `number | 0` caused the last number to jump

## 2.1.0 (May 19th, 2020)

**Big fix:**

- Upgrade use-elapsed-time dependency to v 2.1.2, which fixes and issue with reset method that takes none number values

**Implemented enhancements:**

- The default decimal places count is not determined based on the maximum number of decimal places in `start` and `end`. The decimal places count is also used in `toLocaleString`

## 2.0.0 (May 18th, 2020)

**Breaking Changes**

- The hook now returns an object with two props: `value` and `reset`. `value` is the current count up value; `reset` is a method that reset the animation when it is fired
- The hook now accepts a single object as an argument with all props to configure the animation.

**Implemented enhancements:**

- The library exports also Count up component. The component is using the hook internally.
- Support `toLocaleString` with fallback options
- Add bunch of props to configure the output value
- Rewrite the source code using TypeScript
- Support React Native

## 1.0.4 (Nov 27th, 2019)

**Minor changes:**

- Update TypeScript type definitions

## 1.0.3 (Nov 24th, 2019)

**Minor changes:**

- Update Readme

## 1.0.2 (Nov 24th, 2019)

**Implemented enhancements:**

- Add TypeScript type definitions

## 1.0.1 (Nov 13th, 2019)

**Minor changes:**

- Update .gitignore, .npmignore and Readme

## 1.0.0 (Oct 6th, 2019)

**Implemented enhancements:**

- Init the project with simple hook and returns the count up value