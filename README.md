# Transcript to Meeting Notes

A Codex skill that turns a plain-text meeting transcript into a clean, self-contained HTML meeting record.

The skill extracts meeting metadata, discussion points, confirmed decisions, action items, unresolved questions, and the next checkpoint. It keeps the original transcript unchanged and uses an embedded, responsive HTML template with no external dependencies.

## What it produces

- A single standalone `.html` meeting-notes file
- Clear separation between discussion, decisions, and action items
- Owner, deadline, and status fields for every action item
- Responsive and print-friendly styling
- Output in the transcript's language by default

## Install

Clone this repository into your Codex skills directory:

```bash
git clone https://github.com/Ponti4/transcript-to-meeting-notes.git ~/.codex/skills/transcript-to-meeting-notes
```

Restart Codex if the skill does not appear immediately.

## Use

Attach or provide a local `.txt` meeting transcript and ask:

```text
Use $transcript-to-meeting-notes to turn this transcript into meeting notes.
```

You can also ask for the result in a specific language.

## Repository structure

```text
transcript-to-meeting-notes/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── assets/
    └── meeting-notes-template.html
```

## Privacy

Meeting transcripts can contain personal or confidential information. Review the source and generated notes before sharing them, and avoid committing transcripts or generated notes to this repository.

## License

MIT
