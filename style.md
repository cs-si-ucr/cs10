Uniform style is important for maintainability.
This document contains the style guide for maintaining CS SI handouts.



Section Convention
---

Each section is separated by a header.
To create a header, put the title on one line, and 3 dashes on the next. (see below)

Every header should have 3 blank lines before its title, and one blank line after its dashes.
The only exception is if the file starts with a header.

```
<!-- other stuff -->



Header Title
---

<!-- more stuff -->
```


Text Convention
---

Each sentence goes on its own line.

Inline code is denoted by single backticks.

```
The `string` datatype can hold multiple characters.
To access individual characters in the string, use the `at` member function.
```

Fill-in-the-blank exercises are often useful to review reading concepts.
To achieve this, it is necessary to add a bit of HDML into the markdown document.

Because HTML can be quite messy, the blank with the answer should be put on its own line.
Only punctuation can join blanks on their line.
This is to reduce overall line count, and because lone punctuation is weird.

```
Mitochondria is the
<a style="color:white;border:solid black;border-width:1px">powerhouse</a>
of the cell
```

To reveal the answer, students must highlight the blank.



Content Convention
---

The following rules are suggestions based on what has worked well in the past.
If better ideas come along, the format can be changed.

`cs10`, `cs12`, and `cs14` consist of two parts: a lab and a discussion section.
The lab portion is 2 hours long and the discussion portion is 1 hour long.



TODO: play with mkdocs.yml heirarchy.
Mimick the CS14 page by adding different categories to a single week.

