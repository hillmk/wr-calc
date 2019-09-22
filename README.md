# wr-calc
World Rugby rankings calculator

Development and testing takes place at [`wr-calc-stage`](https://github.com/rawling/wr-calc-stage).  
Changes are pushed to [`wr-calc`](https://github.com/rawling/wr-calc) once stable.

## Release notes

### 0.13.1
- try to handle WR publishing rankings on match days

### 0.13
- Support nominally Away teams playing at home and gaining home advanage, as seen in Pacific Nations Cup 2019

### 0.12
- Support loading multiple pages of fixtures
- Better support when the last ranking date was a long time ago
- Fix scoping issue?

### 0.11
- Support WRU fixture-links by preserving `w` query parameter

### 0.10.0.1
- handle matches with no events

### 0.10
- Add indicator of live score status
- Show kickoffs in browser-local time rather than venue-local time

### 0.9.3
- Fix issue with NHA detection prematurely populating querystring
- Add kickoff and venue for loaded fixtures

### 0.9.2
- Pull live hotfixes from GitHub
- Support WRU with `w` query parameter
- Try to detect NHA from venue country

### 0.9.1
- Upgrade to latest version of Knockout.js
- Performance upgrades

### 0.9
- Share calculations by putting base date and fixture list into query string

### 0.8
- Use Jekyll (gh pages) to enable SASS
- Material redesign
- Responsive - top/bottom on screens that can't fit left/right

### 0.7.2
- Correct sorting of real-life fixtures

### 0.7
- Visual redesign
- Abbreviate longer team names to save space
- Version CSS/JS links to avoid caching older files

Includes re-instating scrolling panes, disclaimer footer, prettier tables, slightly better loading behaviour.

### 0.6
- Load matches between the latest rankings and the next (i.e. a week), including scores
- Use Knockout rather than manual DOM manipulation

Some behaviour has regressed (panes don't scroll separately; autocompletes are now just selects)
but Knockout simplifies the code and gives immediate feedback on changes.

### 0.5
- Detect RWC matches (thanks to [marcoas](https://github.com/rawling/wr-calc-stage/pull/1))
- Change team IDs from name to IDs from API

### 0.4
- Test new staging workflow
- Show separate loading messages for rankings and fixtures
- Use numeric inputs for scores
- Add ability to add rows above loaded fixtures

### 0.3

- Automatically populate with a week of upcoming fixtures (thanks to [marcoas](https://github.com/rawling/wr-calc/pull/2))
- Replace JSONP call for rankings with `$.get` prompted by the above

### 0.2

- Fix issue with columns misaligning after calculating
- Split out JS and CSS into separate files

### 0.1

- Import from http://irbrankingcalculator.azurewebsites.net/ and fix links to be protocol-relative
- Change IRB to World Rugby