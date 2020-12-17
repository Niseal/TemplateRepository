

[Interactive Basic and Extended Markdown Syntax Elements] (https://www.markdownguide.org/cheat-sheet/)

## Cheat Sheet in Short:

## Basic Syntax

These are the elements outlined in John Gruber’s original design document. All Markdown applications support these elements.

### Heading

# H1
## H2
### H3

### Bold

**bold text**

### Italic

*italicized text*

### Blockquote

> blockquote

### Ordered List

1. First item
2. Second item
3. Third item

### Unordered List

- First item
- Second item
- Third item

### Code

`code`

### Horizontal Rule

---

### Link

[title](https://www.example.com)

### Image

![alt text](image.jpg)

## Extended Syntax

These elements extend the basic syntax by adding additional features. Not all Markdown applications support these elements.

### Table

| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |

### Fenced Code Block

```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

### Footnote

Here's a sentence with a footnote. [^1]

[^1]: This is the footnote.

### Heading ID

### My Great Heading {#custom-id}

### Definition List

term
: definition

### Strikethrough

~~The world is flat.~~

### Task List

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media




CheatSheet - Setup Github on Visual Studio Code

Steps:

    Create a directory on the local file system.
    Create a repo on Github.
    Select Clone "Clone or download" on Github, copy the link
    In Visual Studio Code, sect File -> Add Folder to Workspace -> Select the newly created directory
    Select Terminal Window
    In the window, type:

git config --global user.name <github userID>

git clone <URL from github link copied earlier>

That should be all that's required.  any newly created file should be available on github after stage/commit/push.
