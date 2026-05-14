# SNU Student Events

This repository stores public event data for the student events page on
`sysilviakim.github.io`.

Edit `events.yml` to add or update events. Only events with
`status: "published"` appear on the website.

## Event Fields

```yaml
- title: "[사회과학연구원] 월례세미나: 김서영, Keep Winning with WinRed? Online Fundraising Platform as the Party’s Public Good"
  date: "2026-06-02"
  time: "12:30-14:00"
  location: "16B-222"
  organizer: "사회과학연구원"
  description: "https://www.youtube.com/@snuiss"
  status: "published"
```

Optional fields:

- `link`: registration or information URL
- `end_date`: use for multi-day events

Dates should use `YYYY-MM-DD`.

## Publishing Updates

Changes to `events.yml` trigger the website rebuild workflow automatically.

For this to work, this repository needs a repository secret named
`WEBSITE_DISPATCH_TOKEN`. Use a fine-grained GitHub token that has access to
`sysilviakim/sysilviakim.github.io` with repository `Contents: read and write`
permission.
