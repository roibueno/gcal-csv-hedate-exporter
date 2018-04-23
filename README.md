# gcal-csv-hedate-exporter
Simple tool to create valid Google Calendar CSV file for events importing.

This tool is based and on behalf of the source-code of HeDate developed by Daniel Erez:
https://github.com/erezdaniel7/he-date

# Demo
http://roibueno.co.nf/gcal-csv-hedate-exporter/index.html

# Reusable Functions:
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

# Future Milestones:
- Support bulk events adding in on click
- Bugfix on Hebrew characters (Unicode) on event title - being processed as Giberish on the CSV
- Support extended functionality enables by Google Calendar from this link:
https://support.google.com/calendar/answer/37118?hl=iw
- Add feature for monthly events to support event such as Birkat Ha'Levana
- Avoid letting user to inser more futuristic date on startDate than endDate
- Dev.QA (Robustness) + Clean Code
