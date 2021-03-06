---
id: advanced-topics-nested-lists
title: Nested Lists
layout: docs
category: Advanced Topics
next: advanced-topics-text-direction
permalink: docs/advanced-topics-nested-lists.html
---

The Draft framework provides support for nested lists, as demonstrated in the
Facebook Notes editor. There, you can use `Tab` and `Shift+Tab` to add or remove
depth to a list item.

The [`RichUtils`](/docs/api-reference-rich-utils.html) module provides a handy `onTab` method that manages this
behavior, and should be sufficient for most nested list needs. You can use
the `onTab` prop on your `Editor` to make use of this utility.

By default, styling is applied to list items to set appropriate spacing and
list style behavior, via `DraftStyleDefault.css`.

Note that there is currently no support for handling depth for blocks of any type
except `'ordered-list-item'` and `'unordered-list-item'`.
