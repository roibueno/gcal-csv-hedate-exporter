# gcal-csv-hedate-exporter
Simple tool to create valid Google Calendar CSV file for events importing.

This tool is based and on behalf of the source-code of HeDate developed by Daniel Erez:
https://github.com/erezdaniel7/he-date

# Demo
http://roibueno.co.nf/gcal-csv-hedate-exporter/index.html

# Reusable Functionalities:
- ConvertToGregorian() - Converts Hebrew date to Gregorian date.
- formatDate(new Date()) - Converts JS Date() objects into MM/DD/YYYY format.
- exportCSVFile(headers, items, fileTitle) - Creates CSV file by given headers (=titles), items (=rows) and file name.
- getCurrentHebrewYear() - Gets the current Hebrew year by numbers (e.g. 5778).
- $('#allDayEvent').change() - jQuery prepared section for enabled/diasbled input checkbox-dependent

# Used Libraries/Frameworks:
- JS/jQuery-3.2.1
- Bootstrap-4.0.0 
- Font-awesome-4.7.0
- PopperJS, momentJS

# Future Bugfixing:
- Avoid adding ?eventTitle param after form submission in order to avoid bugs when trying to export more than once (sometimes doesn't work). Try changing <form> to <div>
  - Sanity QA for SHANA_MEUBERET/REGULAR: add events to Adar A + B to 2018 & 2019 and check
  - On dropdown: add text "Adar" to "Adar B" so that it will be clear for users what to choose on regular year
  - Modify for loop from 101 iterations to 100, and so on

# Future Milestones:
- Support bulk events adding in on click
- Auto-load CSV file into Google Calendar using OATH, etc.
- Support extended functionality (location/description/private) by Google Calendar from this link:
https://support.google.com/calendar/answer/37118?hl=iw
- Add feature for monthly events to support event such as Birkat Ha'Levana
- Avoid letting user to inser more futuristic date on startDate than endDate
- Dev.QA (Robustness) + Clean Code
