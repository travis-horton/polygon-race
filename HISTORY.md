# Polygon race — what changed, in plain words

This is the whole history of the polygon-race demo, newest first, written for someone who has never seen the code. The demo draws thirteen nested, rainbow-coloured shapes, from a triangle out to a fifteen-sided one, with a white dot racing around each; every dot finishes one side in the same time, so the dots drift in and out of line. It is shown on travish.com, in the Programming section. Every entry is one step that reached the main version: a pull request, or one day's changes on one topic.

**How to read an entry**
- The heading names the change, links to the full technical detail on GitHub, and says when it landed (YY.MMDD.HHMM, Boise time).
- A bigger entry lists its parts underneath; each part's name links to the exact change that made it.
- **New:** something you can see or use · **Fixed:** a problem that no longer happens · **Behind the scenes:** a real change you can't see · **Removed:** something that is gone · **Try it:** where to see it, only when that still works today.
- "(Later replaced …)" means that version is gone and says what took its place.

*Written from the git history on 26.0925 and checked against the code of each day. From then on, each pull request carries its own entry, and it is added here automatically when the pull request merges.*

## June 2024

**Code tidy** · [commit](https://github.com/travis-horton/polygon-race/commit/2b317c9) · merged 24.0606.1258 · v1.0.4
- Behind the scenes: the code was tidied to the website's style checker, with no change to what the demo draws.

## June 2022

**Code tidy** · [commit](https://github.com/travis-horton/polygon-race/commit/21f81b4) · merged 22.0620.1809 · v1.0.3
- Behind the scenes: the code's formatting was tidied to the style rules, with no change to what the demo draws.

**polygon-race #1: the code reorganized** · [PR #1](https://github.com/travis-horton/polygon-race/pull/1) · merged 22.0612.2050 · v1.0.2
- Behind the scenes: the one long drawing routine was split into small named steps (clear the screen, draw each shape, draw each dot) with clearer names, meant to draw exactly as before.
  Try it: open https://www.travish.com/programming/polygon-race

## July 2021

**Ready for the website** · [commit](https://github.com/travis-horton/polygon-race/commit/da29341) · merged 21.0705.1324 · v1.0.1
- Behind the scenes: the demo now makes its own 1200 by 900 drawing area and places it wherever it is asked, the shape the website uses for its demos, instead of drawing on a canvas its own page provided.

**Polygon race begins** · [commit](https://github.com/travis-horton/polygon-race/commit/02675e2) · merged 21.0702.1452 · v1.0.0
- New: a page of nested coloured polygons, from three sides up, each with a white dot running around its edge.
