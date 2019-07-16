# Tech Scandals & Cancel Culture

The larger & longer a company exists the more likely it is to come up against scandals, breaches & backlash of various shapes & sizes. As far as I can tell, no brand has come out of recent memory with a reputation unscathed. I've documented a number of these organizations below to remind myself, & others, that no one/group is perfect.

**scandal.js**
```js
// this script opens searches for all companies listed, referencing "scandal" via duckduckgo
// this opens 20+ new tabs... run at your own leisure/risk
const exec = require('child_process').exec
const brands = `
  Microsoft
  Google
  Amazon
  Facebook
  Apple
  Uber
  Lyft
  IBM
  AirBnB
  Twitter
  Mozilla
  Kickstarter
  NPM
  GitHub
  GitLab
  Twillio
  Reddit
  LinkedIn
  Netflix
  Tesla
  Adobe
  Dropbox
  Snapchat
  Spotify
  Yahoo
  Oracle
  Linux Foundation
  Node Foundation
  Apache Foundation 
`
brands.split('\n').map(b => !!b.trim() && exec(`open https://duckduckgo.com/?q=${b.trim()}+scandal`))
```

**exposing organizations you probably already knew had problems at one time or another...**
```bash
$ node scandal.js
```
