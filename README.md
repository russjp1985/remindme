# remindme
Simple tool for scheduling growl / audio reminders. Requires `php`, `say`, and `growlnotify`.

To create a reminder:

    remindme -w 1pm -m "Call electric company"

Then just make sure you have this in your crontab:

    remindme -d

Running the `-d` process will announce via `say` and `growlnotify` for any reminders scheduled earlier than now.
