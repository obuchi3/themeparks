# Change Log
Key changes to themeparks NPM module.

## v4.0.0

### Changes

* Project refactor - now written in ES6
* Renamed to themeparks

## v3.0.0

* Refactored codebase significantly
* Added SeaWorld parks (including Busch Gardens and Sesame Place)
* Added Universal Studios and Island Of Adventure parks to API
* Setting environment variable "DEBUG=true" will supply better debugging information that we've had in previous versions
* Disney World Florida, Disneyland California, Disneyland Paris, Disneyland Shanghai and Disneyland Hong Kong now share a common codebase.
* (breaking change) GetSchedule is now GetOpeningTimes
* (breaking change) Schedules now return a maximum of one element per day, with "special" opening hours as a sub-object called "special" (eg. Extra Magic Hours)
* (breaking change) Park object names have been renamed
* (breaking change) No longer need to create a new wdwjs() object to start the API, make separate new objects for each park you wish to access
* 3.0.3 added BETA Six Flags support. Some parks do not yet return proper wait time data, see [#12](https://github.com/cubehouse/wdwJS/issues/12)
* 3.0.6 added ride schedules (only for Disney parks) and new status string for each ride wait time entry
* 3.0.7 fixed Tokyo Disneyland ride active status and added updateTime to Tokyo ride outputs (see #17)
* 3.0.10 added Alton Towers to the supported parks
* 3.0.11 added Chessington to the supported parks
* 3.0.12 added Shanghai Disney Resort to the supported parks
* 3.0.14 added Europa-Park to the supported parks
* 3.1.0 fixed Disney API calls with a new client ID

## v2.0.0

* (breaking change) You must now specify "WDWRequests: true" in your setup options if you wish direct access to WDW API function helpers
* Disneyland Paris is now part of the same API service as Disney World Resort and Disneyland California.
* Added Tokyo Disneyland to supported parks
* Added (non-Disney) Universal Orlando parks to supported parks (added: 2.0.4)

## v1.0.0

* (breaking change) Response formats simplified so all parks return same data structure
* Added Disneyland Paris