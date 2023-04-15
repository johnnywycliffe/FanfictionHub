# Editor design

Fanfiction Hub has a built in editor to assist users in making their stories.

## Features

- Importing
  - Copy/paste
  - GDrive
  - File upload
- Image importer
  - Sort images
  - Images can be embedded once uploaded
- Doc manager
  - Sort documents
  - Edit preexisting documents
  - Export documents
  - Document revisions

## Text format

- Markdown
- WYSIWYG (copy/paste)
- HTML

## Sanitization/rating

To avoid allowing harmful code, injections, etc. Documents will be checked over when submitted. During this process, a rating will also be assigned.

The check will search for:
- Profanity
- HTML tags
- SQL/Code snippets
- Words/phrases suggesting sexual activities
- Words/phrases suggesting violence
- Hyperlinks

Hyperlinks are allowed in the text, but discouraged.

The check will notify users of what it finds, why it selected a rating, and allow the user to change the rating if it missed some things. 

Code/HTML tags will be stripped out of the text.
