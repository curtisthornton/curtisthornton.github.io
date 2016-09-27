---
published: true
layout: post
title: New Folder From Selected Filename Script
desc: >-
  An Applescript that takes the currently selected files and creates folders
  with the same name.
proj-num: 2
proj-url: >-
  https://www.dropbox.com/s/a9znjicpk96ws8z/new%20folder%20with%20filename.app.zip?dl=0
---
## Purpose

The purpose of this script is to make it easier to manage files by automatically creating folders with the same name as the filename, and moving those files into that folder.

## Known Issues

Since this is a process that cannot be completed using Automator, this was written in Applescript. So editing the process requires some knowledge of Applescript coding.

## Code

	tell application "Finder"
		set current_folder to folder of front window
		set x to (get the selection) as list
		repeat with i from 1 to the count of x
			set this_file to item i of x
			if i is not 1 then
				set previous_file to item (i - 1) of x
				set prev_ext to cur_ext
				set prev_name to new_name
			else
				set prev_name to ""
			end if
			set cur_ext to name extension of this_file
			set new_name to text 1 thru -((length of cur_ext) + 2) of (name of this_file as text)
			if new_name is not equal to prev_name then
				set new_folder to make new folder with properties {name:new_name} at current_folder
				move this_file to new_folder
			else
				move this_file to new_folder
			end if
		end repeat
	end tell

## [Download](https://www.dropbox.com/s/a9znjicpk96ws8z/new%20folder%20with%20filename.app.zip?dl=1)