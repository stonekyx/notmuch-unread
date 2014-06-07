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

## License

Copyright (C) 2014  David Thompson <davet@gnu.org>

This program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or (at
your option) any later version.

This program is distributed in the hope that it will be useful, but
WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
