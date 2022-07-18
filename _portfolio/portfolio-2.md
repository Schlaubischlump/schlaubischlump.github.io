---
title: "SuggestionPopup"
excerpt: "A simple AppKit suggestion / autocompletion popup for macOS.<br/><img style='width: 500px;' src='https://raw.githubusercontent.com/Schlaubischlump/SuggestionPopup/master/screenshot.png'>"
collection: portfolio
---

[![License: GNU Affero General Public license version 3](https://img.shields.io/badge/License-LGPLv3-blue.svg)](https://opensource.org/licenses/lgpl-3.0)

This is a suggestion popup implementation similar to the one used by the Maps.app on macOS 10.15. It is provided under the GNU Lesser General Public License v3.0. I only tested it on macOS 10.15, 11.0. MacOS 10.13-10.14 could work. I will test this in the future and make it compatible, if required. This software is still in beta.

![](https://raw.githubusercontent.com/Schlaubischlump/SuggestionPopup/master/screenshot.png) 

A Simple location search can be implemented using the following code:

``` Swift
// Keep a reference to the search completer in memory.
var searchCompleter: LocationSearchCompleter!
...
// Somewhere in your constructor create a LocationSearchCompleter with 
// your textField. You can still use the textField delegate !
self.searchCompleter = LocationSearchCompleter(searchField: searchField)
self.searchCompleter.onShow = { ... }
self.searchCompleter.onHide = { ... }
self.searchCompleter.onHighlight = { ... }
self.searchCompleter.onSelect = { ... }
```


For more information check out [the github repository](https://github.com/Schlaubischlump/SuggestionPopup).