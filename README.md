# timezone_sql
SQL database to manage timezone programmatically

Installaion:
1) open the file "timezone.sql"
2) rename the "timezone_bycountry" table as you preferr
2) Run the sql command to create a new table with all the records

Usage:
1) Match the timezones with the specified time of the clients
Use gmt_offset to adjust times in GTM format https://en.wikipedia.org/wiki/List_of_UTC_time_offsets
OR
Use dst_offset to adjust times for Daylight Saving Time https://greenwichmeantime.com/daylight-saving-time/
2) Convert your GMT or DST time if needed (from hours to seconds), with your favourite language
3) Add or remove time (convert it to seconds) from the specified date/time, with your favourite language
4) Manipulate your time and re-convert it from seconds to a date/time

The best use is always to transform the specified date in epoc UNIX and then convert the GMT or DST hours into seconds and do the math operation; the result should be reconverted in a date/time object
