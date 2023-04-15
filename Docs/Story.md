# Story system design

This document outlines the data structure and basic functionality of the stories.

## Stories

- Name
- Rating
- List of tags
- Word count
- Cover image
- Description
- Chapter list
- Comments
- Likes/Dislikes (total)
- Authorized readers (Public, Whitelist, Private)
- Story status (Complete, in-progress)
- Sequels/prequels

### Landing page design

- Display all tags, word count, number of chapters, etc
- Allow users to open spoiler tags
- Allow users to comment
- Allow users to favorite, follow, like or dislike fic
- Allow users to blacklist fic/Author
- Allow user to report fic/author
- Allow user to open chapter 1, latest chapter, or pick from a drop down of all chapters
- Allow user to open entire story at once
- Allow users to download fic as a PDF
- View all images associated with the story

### Tags

Tags are small strings that let a potential reader know what the story's themes, rating, language, etc. Some of the tags are mandatory and may be automatically applied for language or sexual themes.

Tags are color coded by type for easy parsing.

Mandatory tags:
| Name | Description | Options |
| ---- | ----------- | ------- |
| Crossover | Whether story is in one fandom or multiple | Yes/No |
| Fandom(s) | Fandom story is in | Various |
| Rating | Expected maturity level | See rating section |
| Trigger warning tags | Extreme case tags | See section below.

Mandatory tags and some optional tags have descriptions.

Optional tags:
| Name | Description | Options |
| ---- | ----------- | ------- |
| Language | Language the story is primarily written in | List of languages |
| Genre | 2-4 tags describing themes of the story | List og Genres like "hurt/comfort", "Action", "Romance", etc |
| Characters | List of characters in the fic | Various |
| Relationships | Types of relationships representing in the fic | M/F, M/M, F/F, other |
| Pairings | List of Specific pairings | Various | 
| Misc. Tags | Additional tags that the author can write in. Limited to 20 tags. | N/A |

Optional Tags may be marked as spoilers and hidden from default view. 

#### Ratings

- Everyone: No language, suitable for children. Mild, cartoon violence only
- PG: No language, Some topics or violence may not be suitable for all readers.
- Teen: These books are for mature readers aged 13 and up. Items include frequent language, long potentially graphic battle sequences, and some or strong sex innuendos and discussion of sex. 
- Adult: Content may include pornographic sexual content, pervasive language, and realistic violence like torture and prolonged war sequences.

#### Trigger warning tags

These tags are specific items that are specifically called out as a warning to users. 

- Sexual content
- Non-consensual sexual content
- Torture
- Underage
- Prominent Death
- Descriptions of Gore

A user may tag a fic as any multple of the above, as "Chose not to tag", or none.

Note that tagging a fic as "Underage" does not give an author free reign to write underage characters having sex. Please see the abuses sections to know what is allowed and what isn't

## Chapters

Each chapter is a single upload 

- Chapter text
- Word count
- Image data
- Chapter rating
- Comments
- Likes/Dislikes (Not public, for stats)
- Authorized readers (Public, Whitelist, Private)
- Author's notes
- Author's notes location
- End of chapter poll

## Chapter design

- Chapter title
- Chapter text
- Display/hide chapter rating/stats
- Display/hide Author's notes
- Display poll (if enabled)
- Allow users to comment
- Allow users to favorite, follow, like or dislike fic
- Allow users to blacklist fic/Author
- Allow user to report fic/author
- Next chapter, prev chapter, jump chapter

## Collections

Collection provide a list of stories so a user can keep track of multiple "books" that have a commonality. Collections are at a user's discretion and are not required to follow any logic.

- Description
- Owner
- List of Stories

## Fandoms

Each fandom created as some data associated with it. This data is updated as users create stories, and is provided to make tagging more consistent.

- Name
- Media type (Anime, Book, TV, etc.)
- Characters (OC, Self insert added by default)
- Pairings and pairing type

## Creating a new story

- Author signs into account
- Selects "New Story"
- Selects crossover or not
- Finds fandom(S) 
  - By name
  - If name isn't found, suggest similar names in case of typo or incomplete title
  - Can narrow down by TV, Book, Anime, Game, Etc
- Select rating
- Set visibility 
- Upload first chapter (See uploading a new chapter)
- Add optional tags
  - Pairings, characters and the like are suggested based on story.
- Add description
- Add images
- Publish (Only available after all mandatory options are filled)

New stories can be saved before being published to allow for stories to be generated piecemeal. 

## Uploading a new chapter

- Select saved chapter, or use editor to create new chapter
- Choose chapter title
- Choose chapter rating (Autodetect curse words, sexual themes, violence if possible)
- Add new tags as appropriate
- Embed images as appropriate

## Updating a pre-existing chapter

- Select chapter to update
- Use editor to update chapter, save a copy
- Choose whether to notify readers of change or not.

