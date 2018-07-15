# [NodeSchool](https://github.com/stathoula/nodeschool.github.io) Event Calendar 
Within the course "Software Engineering in Practice", we were assigned to contribute to an Open Source Project from Github.
The project that I decided to contribute to, is [NodeSchool](https://nodeschool.io), which is an [open source project](https://github.com/nodeschool/nodeschool.github.io) run by volunteers with two goals: to create high quality programming curriculum and to host community learning events all around the world. Those events were displayed in a calendar that was looking a bit off, so I decided to improve it.

<img src="https://github.com/stathoula/NodeSchool_Event_Calendar/blob/master/oldCalendar.PNG"> <br>
In order to produce the new calendar I used:
- [FullCalendar](https://fullcalendar.io/), a customizable and open source project javascript event calendar. 
- [Tabletop.js](https://www.npmjs.com/package/tabletop), which takes a Google Spreadsheet and makes it easily accessible through JavaScript. *The nodeschool's events are hosted in [this](https://docs.google.com/spreadsheets/d/1swvC909BzbpToZLePM6whDvmXavaxEG6eT257dVf-bY/pubhtml) public spreadsheet.*

After writting the appropriate code, the result was this:

<img src="https://github.com/stathoula/NodeSchool_Event_Calendar/blob/master/newCalendar.PNG">

My [pull request](https://github.com/nodeschool/nodeschool.github.io/pull/616) was merged :tada: :tada: 
You can find the calendar [here](https://nodeschool.io/events.html)!

### Code Structure 
- ["Lib" Folder](https://github.com/stathoula/NodeSchool_Event_Calendar/tree/master/lib) contains the files needed in order to use [FullCalendar](https://fullcalendar.io/).
- ["eventCalendar.js"](https://github.com/stathoula/NodeSchool_Event_Calendar/blob/master/eventCalendar.js) contains the code that I wrote in order to parse the events from the [public spreadsheet](https://docs.google.com/spreadsheets/d/1swvC909BzbpToZLePM6whDvmXavaxEG6eT257dVf-bY/pubhtml) to the callendar using tabletop.js.
- ["eventCalendar.html"](https://github.com/stathoula/NodeSchool_Event_Calendar/blob/master/eventCalendar.html) display the calendar.

> The code is adjusted to the needs of Nodeschool. 
> However, it might help someone that wants to build 
> a calendar that takes the events from a public spreadsheet.
