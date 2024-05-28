# Heading 1

## Heading 2 text

Hello world!
We will output Markdown to:

- HTML
- docx
- PDF

Link to [Google](http://www.google.com/)

```javascript
// this is a code sample\
import React from 'react';

const test = () => {
	return <div>test</div>;
};

export default test;
```

Here's a list:

1. First ordered list item
2. Another item
   - Unordered sub-list.
3. Actual numbers don't matter, just that it's a number
   1. Ordered sub-list
4. And another item.

   You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

   To have a line break without a paragraph, you will need to use two trailing spaces.
   Note that this line is separate, but within the same paragraph.
   (This is contrary to the typical GFM line break behavior, where trailing spaces are not required.)

- Unordered list can use asterisks
  + Or pluses
    - Or minuses

But we should use consistent formatting in lists because it's easier to read:

* Unordered lists
  + should use
    - consistent formatting
  + in sublists
* and their roots
