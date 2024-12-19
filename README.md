# FilterBugList plugin for MantisBT

By Alain D'EURVEILHER (alain.deurveilher@gmail.com).

## Description

Plugin for MantisBT allowing to filter by a set of bug IDs in the *View all* page.

## Requirements

- MantisBT 2.x

## Usage

A new *Bug List* filter field is available on the View Issues page's Filters section.

The filter can accept any kind of bug list as a string, using any non-numeric
character as a separator.

For instance: 
`5079, #5073-5108 5107 49396{5006}}`
will result in a filtering of the following bug IDs: 
*5079, 5073, 5108, 5107, 49396, 5006*.

The filter is also accessible via the FilterBugList_list query in the url,
for instance:
http://example.com/mantis/view_all_set.php?type=1&temporary=y&FilterBugList_list=5079,5073,5108,5107,49396,5006


## Support

Use [GitHub Issues](http://github.com/mantisbt-plugins/Announce/issues).


## Changelog

### 2.1.1 - 2024-12-19
- Fix deprecation warnings #3 #4
- Code cleanup

### 2.1.0 - 2017-01-24
- Compatibility with Mantis 2.0.0

### 2.0.0 - 2016-10-27
- Compatibility with Mantis 1.3.0

### 1.0.0 - 2014-12-05
- Creation of the plugin
