# notmuch-unread

A global minor mode that displays the number of unread messages in the
notmuch database in the mode line.

## Installation

```lisp
(add-to-list 'load-path "/path/to/notmuch-unread")
(require 'notmuch-unread)
```

## Usage

`M-x notmuch-unread-mode`

The unread message count is displayed next to the ✉ character in the
mode line.

## Customization

By default, notmuch-unread counts the number of messages with the
'unread' tag.  This can be changed by customizing
`notmuch-unread-search-term` to a notmuch search term of your liking.

The default update interval is 5 seconds.  Customize
`notmuch-unread-update-interval` to change this.