# Readme.md

This is an attempt at copying [https://julialang.org]() using Franklin.jl.

## How to maintain this

Clone the repository, `cd` to it, and, in Julia, assuming you have Franklin do `using Franklin; serve()` then go to `localhost:8000` on your browser and edit away.

## Link checks

* [x] page `/benchmarks/` is missing
* page `/platform/` is missing
* page  `projects/` `guidelines/` `archives/`
* 2019 multithreading blog needs checks

## Notes

**todo**
* nightlies page [this one](https://julialang.org/downloads/nightlies)
* old release page [this one](https://julialang.org/downloads/oldreleases)
* diversity page [this one](https://julialang.org/diversity)
* fixed assets like [this one](https://julialang.org/images/2019-julia-user-developer-survey.pdf)
* lazy subpages (copy-paste html)
* some internal links may be erroneous (H* links are slightly different now)
* some  links with `julialang` in them link should be fixed
* some leftover `{{page.manurl}}` or related
* [x] styling on blog page to have dates on other line
* [x] add link to Franklin in footer

**notes**

* dumped a bunch of `<head>...</head>` statement (index.html)
* ~~need to check the scripts, put the relevant assets (e.g. bootstrap) in appropriate places~~
* ~~check index html then other~~
