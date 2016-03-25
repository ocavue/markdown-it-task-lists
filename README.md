# markdown-it-task-lists

A [markdown-it](https://www.npmjs.com/package/markdown-it) plugin to create GitHub-style [task lists](https://github.com/blog/1825-task-lists-in-all-markdown-documents)

[![Code Climate](https://codeclimate.com/github/revin/markdown-it-task-lists/badges/gpa.svg)](https://codeclimate.com/github/revin/markdown-it-task-lists)

## What it does

- Builds task/todo lists out of markdown lists with items starting with `[ ]` or `[x]`.
- Nothing else

### Why is this useful?

When you have markdown documentation with checklists, rendering HTML checkboxes
out of the list items looks nicer than the raw square brackets.

## Installation

```sh
npm install markdown-it-task-lists
```

## Usage

Use it the same as a normal markdown-it plugin:

```js
var md = require('markdown-it');
var taskLists = require('markdown-it-task-lists');

var parser = md().use(taskLists);

var result = parser.render(...); // markdown string containing task list items
```

## Tests

```sh
npm install
npm test
```

## License

ISC