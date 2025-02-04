# DateUtils Library

## Description
A Python python-datetimehelper library for working with dates, time formatting, and timezone conversions.

## Installation
```bash
pip install python-datetimehelper
```

Usage
1. Importing the Library
You can import the DateUtils class from the package and start using its methods.

Example :


```bash
from datetime_helper import DateUtils

```
2. Formatting Dates
The format_date method allows you to format a datetime object or an ISO 8601 string into a custom date format.

Example :

```bash
from datetime import datetime
from datetime_helper import DateUtils

date_input = datetime(2024, 11, 20, 14, 30, 00)
formatted_date = DateUtils.format_date(date_input, 'dd-MM-yyyy HH:mm:ss')
print(formatted_date)  # Output: 20-11-2024 14:30:00
```

3. Converting Timezones
The convert_timezone method enables you to convert a datetime object from one timezone to another.

Example :

```bash

from datetime_helper import DateUtils
from datetime import datetime

date_input = datetime(2024, 11, 20, 14, 30, 00)
converted_date = DateUtils.convert_timezone(date_input, 'UTC', 'Asia/Kolkata')
print(converted_date)  # Output: 2024-11-20 20:00:00+05:30

```

4. Adding Time
You can add or subtract time (days, hours, minutes, etc.) to a datetime object using the add_time method.

Example:

```bash

from datetime_helper import DateUtils
from datetime import datetime

date_input = datetime(2024, 11, 20, 14, 30, 00)
new_date = DateUtils.add_time(date_input, days=2, hours=5)
print(new_date)  # Output: 2024-11-22 19:30:00

```

## Documentation

For more detailed usage and additional features, refer to the [documentation on GitHub](https://github.com/kiraningale012/python-datetimehelper).

## Sources and References

- [Python datetime documentation](https://docs.python.org/3/library/datetime.html)
- [pytz library documentation](https://pypi.org/project/pytz/)