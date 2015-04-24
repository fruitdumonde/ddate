DDate
=====

[![Build Status](https://travis-ci.org/a-tal/ddate.png?branch=master)](https://travis-ci.org/a-tal/ddate)
[![Coverage Status](https://coveralls.io/repos/a-tal/ddate/badge.png?branch=master)](https://coveralls.io/r/a-tal/ddate?branch=master)
[![Stories in Backlog](https://badge.waffle.io/a-tal/ddate.png?label=ready&title=Backlog)](https://waffle.io/a-tal/ddate)
[![Stories In Progress](https://badge.waffle.io/a-tal/ddate.png?label=ready&title=In+Progress)](https://waffle.io/a-tal/ddate)
[![Version](https://pypip.in/v/ddate/badge.png)](https://pypi.python.org/pypi/ddate/)
[![Downloads this month](https://pypip.in/d/ddate/badge.png)](https://pypi.python.org/pypi/ddate/)

Discordian Date Python Object Class.


Python Usage Examples
=====================

```python
>>> from ddate import DDate
>>>
>>> DDate()
<src.ddate.DDate object at 0x7f3a6b88eb50>
<DDate date: 2014-02-01, day_of_season: 32, day_of_week: 1, holiday: None, season: 0, year: 3180>
>>>
>>> print(DDate())
Today is Boomtime, the 32nd day of Chaos in the YOLD 3180
>>>
>>> import datetime
>>> print(DDate(datetime.date(year=2014, month=4, day=20)))
Setting Orange, the 37th day of Discord in the YOLD 3180
```

Command Line Examples
=====================

```bash
$ ddate
Today is Pungenday, the 40th day of Discord in the YOLD 3181

$ ddate --help
usage: ddate [day] [month] [year]

$ dcal
 Discord 3181 
Sw Bo Pu Pr Se
71 72 73  1  2
 3  4  5  6  7
 8  9 10 11 12
13 14 15 16 17
18 19 20 21 22
23 24 25 26 27
28 29 30 31 32
33 34 35 36 37
38 39 40 41 42
43 44 45 46 47
48 49 50 51 52
53 54 55 56 57
58 59 60 61 62
63 64 65 66 67
68 69 70 71 72
73  1  2  3  4

$ dcal --help
Similar to the `cal` command, but for the Discordian calendar.

Usage:
    dcal [season] [year]

Season can be an integer between 1 and 5, steps with + or -, 'next', or any of
the Discordian season names. The year is in Discordian (+= 1166 to Gregorian).

Examples:
    dcal +2          # prints two seasons into the future
    dcal aft         # prints the last season (The Aftermath) of this year
    dcal discord -2  # prints the Discord season from two years ago
    dcal +6 +1       # prints the calendar 6 seasons and one year in the future

Discordian season names:
    Chaos
    Discord
    Confusion
    Bureaucracy
    The Aftermath
```

Install
=======

Simple way:
```bash
$ pip install -U ddate
```

Or from source:
```bash
$ git clone https://github.com/a-tal/ddate
$ cd ddate
$ python setup.py install
```

Live Demo
=========

![live demo gif](https://github.com/a-tal/ddate/raw/gh-pages/images/ddemo.gif)
