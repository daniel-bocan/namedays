# Name Days

This repository contains JSON calendars of name days for various countries.

These datasets were compiled by cleaning, parsing, and combining data from multiple internet sources, Wikipedia, and open community repositories. Due to the complex nature of local traditions and conflicting sources, these datasets are provided "as-is" and may contain errors, inaccuracies, or missing information.

I highly welcome any contributors who want to correct and improve these datasets via Pull Requests.

## General formatting

- **Static calendars**: The key is the date in the `MM-DD` format.
- **Movable calendars**: The key is the integer offset (in days) from Orthodox Easter Sunday.
- **Christmas calendar (`gr_christmas.json`)**: This dataset contains only two entries with `sunday_of_forefathers` and `sunday_before_christmas` keys. These name days belong to the Sundays before Christmas. Christmas is fixed (December 25th), but these Sundays fall on different dates each year.
- **Empty dates**: If there are no names on some date, the date is excluded from dataset.

## Dataset-Specific Notes

### Latvia (`lv.json`)

- `05-22`: Traditionally designated as the name day for all people whose names are not officially listed in the calendar (often displayed in local calendars with the phrase "Visi kalendāros neierakstītie vārdi").

### Greece (`gr_static.json`)

Greek name days follow specific shifting rules based on Orthodox Easter:

- If Orthodox Easter Sunday falls on or after `04-23`: Name days on `04-23` are moved to Easter Monday (offset `+1`).
- If Orthodox Easter Sunday falls on or after `04-25`: Name days on `04-25` are moved to Easter Tuesday (offset `+2`).

## Disclaimer

The data and files in this repository are provided **"as is", without warranty of any kind**, express or implied. You are free to use, modify, and distribute these datasets in your own applications.
