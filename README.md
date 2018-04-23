# gcal-csv-hedate-exporter
Simple tool to create valid Google Calendar CSV file for events importing

This tool is based on the source-code of HeDate developed by Daniel Erez:
https://github.com/erezdaniel7/he-date

# Future Milestones:
- Support bulk events adding in on click
- Bugfix on Hebrew characters (Unicode) on event title - being processed as Giberish on the CSV
- Support extended functionality enables by Google Calendar from this link:
https://support.google.com/calendar/answer/37118?hl=iw
- Add feature for monthly events to support event such as Birkat Ha'Levana
- Avoid letting user to inser more futuristic date on startDate than endDate
- Dev.QA (Robustness) + Clean Code
