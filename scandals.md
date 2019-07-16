# Tech Scandals & Cancel Culture

No one is perfect. The larger & longer an organization exists the more likely it is to come up against the will & moral high-ground of the masses. Scandals, breaches & backlash take all shapes & sizes; No tech company has come out of recent memory with a reputation unscathed. I've documented a number of these companies below for my own sanity.

**scandal.js**
```js
// this script opens searches for all companies listed, referencing "scandal" via duckduckgo
// this opens 20+ new tabs... run at your own leisure/risk
const exec = require('child_process').exec
const companies = `
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
  Yahoo
`
companies.split('\n').map(c => !!c.trim() && exec(`open https://duckduckgo.com/?q=${c.trim()}+scandal`))
```

**exposing companies, you probably already knew had problems at one time or another...**
```bash
$ node scandal.js
```
