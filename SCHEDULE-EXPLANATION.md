# Schedule Explanation

The GitHub Actions workflow for our Daily Pennsylvanian scraper is configured to run automatically based on three triggers:

1. When code is pushed to the main branch
2. When a pull request is made to the main branch
3. On a daily schedule defined by the cron expression: `"0 20 * * *"`

The cron expression can be broken down as follows:
- `0` - At minute 0
- `20` - At hour 20 (8:00 PM UTC)
- `*` - Every day of the month
- `*` - Every month
- `*` - Every day of the week

This means our scraper automatically runs once per day at 8:00 PM UTC (3:00 PM EST during standard time, 4:00 PM EDT during daylight savings). This timing was chosen to capture the day's top sports headlines when most of the day's content has been published but before the evening updates.

You can use [crontab.guru](https://crontab.guru) to experiment with and verify cron expressions.
