# SNU Student Events

This repository stores public event data for the student events page on
`sysilviakim.github.io`.

Edit `events.yml` to add or update events. Only events with
`status: "published"` appear on the website.

## Event Fields

```yaml
- title: "GRE Writing 워크샵"
  date: "2026-06-22"
  time: "09:30-12:00"
  location: "16-315"
  organizer: "김서영(교수)"
  description: "GRE 글쓰기의 기초와 첨삭"
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
