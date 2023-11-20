# MostActiveCookie

MostActiveCookie is a command line program in Python to process the log file and return the most active cookie for specified day. This was a project proceeded for Quantcast.

In order to run this program, you will need a csv file with cookie and timestamp inside. The example for csv will be like following:

```
Cookie,Timestamp
AtY0laUfhglK3lC7,2018-12-09T14:21:00+00:00
AtY0laUfhglK3l67,2018-12-09T14:20:00+00:00
```

You would need Python with version at least `3.8` and csv file that includes appropriate cookie and timestamp with header.

## Quick Start

<b>Scenario: Extract Most Active Cookie in 2018-12-09.</b>

You can either use pip install, or just clone repository itself.

### Use pip install

```bash
> pip install most-active-cookie
> python3 -m most_active_cookie your_cookie_file.csv --date 2018-12-09
> AtY0laUfhglK3lC7
> AtY0laUfhglK3l67
```

### Clone repository

```bash
> git clone https://github.com/yongchand/MostActiveCookie.git && cd MostActiveCookie
> python3 -m most_active_cookie your_cookie_file.csv --date 2018-12-09
> AtY0laUfhglK3lC7
> AtY0laUfhglK3l67
```

## Testing

Test can be performed using pytest

```bash
> pytest -v 
> cd tests/jobs #only when previous command does not work
> python3 -m pytest #only when previous command does not work
```

## Future Works
- Add support to other file formats
- Add alert for cookie input
- Consider adding logging