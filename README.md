# Chronolog
_Format spec for logging daily activities._

_Chronolog_ is a markup language based on [Markdown](https://en.wikipedia.org/wiki/Markdown) developed to enable easy and smart daily activities logging. You can write your own diary in plain text into single text file. It's fast, easy and universal. Chronolog file is a valid .md file with a multiple additional conventions like `tags`, `day items`, `activities` etc. Due to well defined syntax it's open for many useful tools like writing assistants, automatic analyzers, mobile apps etc. Feel free to try it and share your experiences and preferences.

## Example
```
## Sa 2016-12-31
* 08.00: Breakfast with @Jane at #home.
* 10.00 - 11.00: Starting my new project Chronolog.
* 11.00 - 12.00: Lunch with @Lucy in #Royal_Caffe.
* 14.00 - 16.00: Playing football with my friends. #sport #long_street

## Fr 2016-12-30
Long sleeping. Playing Carcassonne with @John and @Jack.
```

### Explanation
* __Day item__ is a basic Chronolog "building stone". It's a text block starting with `## WD YYYY-MM-DD` title. Note, that two day-name sets are supported: czech (Po, Út, St, Čt, Pá, So, Ne) and english (Mo, Tu, We, Th, Fr, Sa, Su). Day items are divided with at least single empty line.
* __Activity__ is represented with a single line contained in the day item. It can start with __clock__ point (08.00) or __clock line__ (09.00 - 10.20).
* __Tag__ is a single unique word starting with #. It's useful for frequently used themes, places etc.
* __Person__ is a single unique word starting with @ meaning concrete person.
