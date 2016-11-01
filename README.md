# slate-edit-footnote

[![NPM version](https://badge.fury.io/js/slate-edit-footnote.svg)](http://badge.fury.io/js/slate-edit-footnote)
[![Linux Build Status](https://travis-ci.org/GitbookIO/slate-edit-footnote.png?branch=master)](https://travis-ci.org/GitbookIO/slate-edit-footnote)

A Slate plugin to handle footnote edition.

### Install

```
npm install slate-edit-footnote
```

### Features

- Normalize footnotes to be at end of the document

### Simple Usage

```js
import EditFootnote from 'slate-edit-footnote'

const plugins = [
  EditFootnote()
]
```

#### Arguments

- ``[typeFootnote: String]`` — type for the footnote block
- ``[typeRef: String]`` — type for the footnote ref

### Utilities and Transform

`slate-edit-footnote` exports utilities and transforms:


#### `transforms.insertFootnote`

`plugin.transforms.insertFootnote(transform: Transform) => Transform`

Insert a new empty footnote, with a reference at the current position.