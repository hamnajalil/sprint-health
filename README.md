# Sprint Health

**Drop a Jira export, get a sprint health check and a paste-ready status update. Thirty seconds, no login, nothing leaves your browser.**

**Try it: [hamnajalil.github.io/sprint-health](https://hamnajalil.github.io/sprint-health/)** (click *Try it with sample data* if you don't have an export handy).

## Why

Every sprint review asks the same questions: are we on pace, what got carried over again, what was added halfway through, who is overloaded, what has gone quiet. Jira can answer each of them, but across five boards and three filters, and never in a form you can paste into a status update.

This page answers all of them from the one export Jira already gives you.

## How to use it

1. In Jira, open your sprint's issues and choose **Export → CSV (all fields)**.
2. Open the page and drop the file on it.
3. Read the verdict, then copy the status update at the bottom.

That's it. Nothing is uploaded. The file is read inside your browser and never sent anywhere.

## What you get

- **A verdict:** on track, at risk or off track, with the reasons.
- **Six numbers:** done, in progress, carried in from earlier sprints, added mid-sprint, blocked, and gone quiet (in progress with no update in over five days).
- **What to look at:** plain-language warnings, such as issues that have been in three or more sprints, or one person holding most of the open work.
- **Carried-over issues**, with how many sprints each has been in.
- **Who's carrying what:** done and open work per person.
- **A status update** in plain text, ready for Slack or email, with a Copy button.

## What it reads

The page looks for these columns and copes if some are missing: issue key, summary, issue type, status (and status category), assignee, created, updated, resolved, every `Sprint` column, story points, and any `Flagged` column. Pick a sprint and set the start date and length to get the pace check.

## Limits

- **Added mid-sprint is partial.** It counts issues created after the sprint start. An older issue dragged into the sprint late won't show, because the export doesn't record when that happened.
- **Jira exports vary** between companies. If yours doesn't load, [open an issue](https://github.com/hamnajalil/sprint-health/issues) and attach a few rows with the sensitive bits removed.

## Run it yourself

It's one HTML file with no dependencies. Download `index.html` and open it, or host it anywhere static files go.

## Who made this

[Hamna Jalil](https://hamnajalil.com), technical PM and game producer. I built this because I kept doing this count by hand on Friday afternoons. See also the [AI Project Kit](https://github.com/hamnajalil/ai-project-kit).

## License

[MIT](LICENSE).
