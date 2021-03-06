Export plugin for Craft CMS
=================

Plugin that allows you to export data to CSV files.

Features:
- Export Entries and Entry Types (All types or per type)
- Export Users and User Groups
- Export Categories
- Sortable export field order
- Renameable column labels
- Ability to save your sort and column settings
- Has a hook "registerExportSource" to add/replace exports with your own source.
- Has a hook "registerExportOperation" to parse special export fields

Todo:
- Export all ElementTypes (currently only Entries, Users and Categories)
- Support JSON and XML output
- Permissions, who can export what

Important:
The plugin's folder should be named "export"

Changelog
=================
###0.4.5###
- Added getCsrfInput function to forms

###0.4.4###
- Even better field data parsing

###0.4.3###
- Better field data parsing

###0.4.2###
- Fixed a serious issue that led to not being able to run Export independently from Import

###0.4.1###
- Added a hook "registerExportOperation" to parse special export fields

###0.4.0###
- Added the ability to export parents and ancestors
- Added the ability to pick your own column names
- Added the ability to save column names and order
- You can also clear this (with permission to "reset")
- Fixed a lot of bugs with multiple title columns
- Only escape double quotes in CSV
- Ability to export fields that return an array

###0.3.2###
- Allow multiple title columns when exporting multiple entry types

###0.3.1###
- Added the ability to export all entrytypes in a section at once

###0.3.0###
- Added the ability to export Categories
- Added the ability to sort the export field order

###0.2.4###
- Added the ability to export id's

###0.2.3###
- Fixed wrong parsing of Lightswitch values
- Fixed skipping of existing columns with NULL values

###0.2.2###
- Mostly common bugfixes and improvements

###0.2.1###
- Fixed a bug that would compromise exportSource data when multiple hooks were used

###0.2###
- Added a "registerExportSource" hook, so you can replace/add/delete export data from your own plugin

###0.1###
- Initial push to GitHub