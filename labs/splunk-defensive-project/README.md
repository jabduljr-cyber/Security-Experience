# Defensive Security Project: Splunk Log Analysis

For this bootcamp project I used Splunk to analyze Windows and Apache logs from a fictional company, comparing a normal baseline day with a day when an attack took place. The data came from a training exercise.

## What I did
- Installed the Splunk Add-On for Unix and Linux
- Built reports for Windows (signatures, severity levels, success rate) and Apache (HTTP methods, top referrers, response codes)
- Created alerts with baselines and thresholds, including failed activity, hourly logins, account deletions, non-US traffic, and HTTP POST spikes
- Built dashboards and compared them against the attack-day logs

## What I found
- Windows: high-severity events rose from about 6% to about 20%, with spikes in account lockouts and password-reset attempts and a login spike in the late morning
- Apache: a large jump in HTTP POST requests, more 404 responses, a spike in traffic from Ukraine, and the logon page was the most requested page
- Together this looked like a brute-force attack on the logon page

## What I'd recommend
Rate limiting on the logon page, account lockout, MFA, and blocking suspicious sources.

## What I learned
My alert thresholds were set too low compared with the real attack counts. I'd tune them using more baseline data so alerts catch attacks without firing on normal days.

[Read the full report (PDF)](rekall-pentest-report.pdf)
