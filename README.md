![Mastodon](https://i.imgur.com/NhZc40l.png)
====

View the documentation at <https://docs.joinmastodon.org>

### Build/Deploy

#### Requires
* Hugo (on macOS: `brew install hugo`)


#### build the static site
`hugo -D` 

Output will be in `./public/` 

TODO clean up the ad hoc quick and dirty doc copy, for now:

`cp ./public ../public/docs`
`cp ./public/docs ../public/docs`

This hack will copy the static files into ../public/docs, and then copy the ./public/docs/ folder content into ../public/docs as well so we can route to the static files properly (There is 100% an easy fix that will allow for this hack to be removed, but for now it works.)