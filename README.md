# Kansas City FGC Community Resources

## Contributing

Even if you are not a developer, adding pages to this website is incredibly simple! All of the content in this website is generated using the Markdown files contained within this repository, which are simple text files with additional syntax for basic formatting. If you've formatted messages in Discord before, you're already familiar. A more comprehensive description of Markdown formatting is available at [markdownguide.org](https://www.markdownguide.org/cheat-sheet/).

### Creating an event

1. Copy the contents of [archetypes/events.md](https://raw.githubusercontent.com/kc-magic-pixel/kc-magic-pixel.github.io/main/archetypes/events.md) to your clipboard.
1. Create a new file in [content/events](https://github.com/kc-magic-pixel/kc-magic-pixel.github.io/new/main/content/events), and name the file with the format `YYYY-MM-DD-name-of-event.md`.
1. Paste the archetype into the newly created file, and replace all fields in the "front matter" (the section surrounded by `---`).
    - You may remove any properties that aren't relevant to you, except for lines that say `# required` at the end.
1. In the top right, click "Commit changes", and in the dialog that appears select "Create a new branch for this commit and start a pull request".
1. A reviewer will look over your submission. Once accepted, it'll go live on the website immediately.

### Modifying the schedule

1. Open the [schedule.yaml](./data/schedule.yaml) file.
1. Each of the items in `games` is a game name as it appears in start.gg. The `schedule` property of each game is dictionary where the keys are event names (as they appear in the website, check the [series pages](./content/series/)), and the values are the week of the month where that occurs.
    - For example, `3` indicates the 3rd week of the month, on the weekday that the event occurs.

## Development

This section is only relevant if you are working on site functionality or layout.

1. Install the [Hugo CLI](https://gohugo.io/getting-started/quick-start/).
