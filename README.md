# exercise: positioning

source: https://courses.joshwcomeau.com/css-for-js/02-rendering-logic-2/11-exercises-pt-2

issues to fix per video:

- sidebar should go beneath header, not above
- loading spinner should go beneath header, not (partly) above
- help icon should go above sidebar, not beneath it

in a nutshell: all the layers are out of order!

guide to files:

- GlobalStyles: ignore
- App.js: heart of things
- LoadingSpinner: don't touch it; pretend it's an external dependency
- PageContent: puts together Sidebar, MainContent (defined in PageContent file), and LoadingSpinner

# notes

- whoa that's a lot of `npm i` spew about missing peers and outdated versions.
- there wasn't any package.lock to begin with.
