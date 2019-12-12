# Markdown Tag Organizer

This is a tool to let you organize, view, and edit all of your markdown notes by tag.

I'm fed up with current note-taking applications. I want a system where
1. Notes are stored as text on my system
2. I can write in vim
3. I can quickly view/edit all notes of a particular tag
4. add more

This is meant as tool to fill the gap in vim-enthuasiast developers

Usage:

```
./buildTagList exampleNotes/ apple
# produces apple.mdtl
```

This will search all markdown notes in the specified directory and concatenates notes matching the tag into a .mdtl file. Markdown files match the tag if they have a YAML metadata block present, a `tags:` field, and the specified tag listed with a ` - ` under that field.
