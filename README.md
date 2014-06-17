helpfulscripts
==============

A collection of helpful scripts that make working in Linux easier


DBUS-aware Scripts:
* cron-notify: send messages via notify-send, even from cron
* telepathy-presence: set status on all telepathy (empathy) accounts
* purple-status: set status in Pidgin and any libpurple-based IM client

These scripts all check for a 'dbus-daemon' running, and grab $DBUS_SESSION_BUS_ADDRESS from its environment.  With that variable defined, they can all interact via DBUS, even from a cron job or a remote SSH session.  I use them in cron jobs to automatically sign in and out of IM and send libnotify notices.

Helpful extras:
* tea-timer: a simple timer that uses zenity to count down and notify you when the timer expires
* oom-scores: Shows the processes that are most likely to be culled by the OOM-killer
