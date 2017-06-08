# nagios-check\_log\_count

## Usage

```
check_log_count [-w warning_th] [-c critical_th] [-t tmpfile] -l target_log
```

Example:

```
check_log_count -w 5 -c 10 /tmp/error_log_count -l /var/log/error.log
```

When tmpfile not set, use `/tmp/check_log_count_(MD5 of target_log)` by default.

If you want to ignore specific line. Edit it.

```
# ignore patterns
patterns = [
  %r(INFO ),
]
```

