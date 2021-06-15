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

# notes from getting started

- whoa that's a lot of `npm i` spew about missing peers and outdated versions.
- there wasn't any package.lock to begin with.

# notes after watching solution video

- ok, apparently Help going under the app bar could maybe not be OK if you stuck it over the app bar, but that's also going to go over your login widget or whatever, so please don't do that.
  - my first thought was "hey let's isolate that other crud", so i'm confident i would have arrived at basically the same solution. the isolate + dom order combo is such a great tool to have in my toolbox!
- isolating the whole target element we're rendering into so that portals will wind up atop it and not fighting for z-index? i love it.
