# xcsoar-data-content

## Folder structure and where to put what
	
	* airspaces
		- airspace files for each country
		- special: special airspace files like thermal hotsports, wave areas, etc.
	* scripts
	* waypoints
		- airfield: files with airfields and maybe UL strips for each country
		- outlanding: files with outlanding strips for each country (maybe UL strips should be put in here?)
		- special: files with special waypoints like thermal information, etc.
		- turnpoint: files with turnpoint information (no airfields, outlanding strips, special data, etc.)
			- events: turnpoint files generated for events like competitions, etc.

All original files (just the country name, nothing else) which are not using the new name scheme should be considered as depricated. These files need to be splittet (because they contain airfield, turnpoint, outlanding data all in one file) in new files (one file containing only one kind of waypoint data) and checked (double entries, updates available, etc.).

## Country Codes and Country Names for Filenames

Country codes and names used in filenames are according to ISO-3166 Alpha-2 standard. Have a look at the folling link:
[Wikipedia ISO 3166-1](https://en.wikipedia.org/wiki/ISO_3166-1)

## SVN Setup

To use the automatic SVN Keyword Substitution (for Metadata in File Headers) please have a look at the following link and configure your SVN client accordingly.
[How To Use SVN Keyword Substitution with TortoiseSvn](https://sfriederichs.github.io/how-to/svn/2017/12/01/SVN-Keyword-Substitution.html)
This seems to be not working with GitHub. Maybe there is another possibility to do this with GitHub?

## To-Do and Ideas

	* Improve readme
	* Create script for automatic file downloading where possible (e.g. TravelByGlider)
	* Fix Metadata in File Headers automatic generatio via Keywords

# Readme from original GitHub Repository (Not everything mentioned here is correct for my new created forked repository)

[![Travis Build Status](https://img.shields.io/travis/XCSoar/xcsoar-data-content/master.svg)](https://travis-ci.org/XCSoar/xcsoar-data-content)
The data here is made available at [download.xcsoar.org](http://download.xcsoar.org).

It currently maintains:
 * Waypoint files that contain:
   - Turn-points
   - Airfields
   - Out-landing Sites
 * Airspace files:
   - Airspaces that have no other source

## Contributions
Contributions here have to pass:
- A review by another contributer
- A parsing check by [aerofiles](https://github.com/Turbo87/aerofiles)

They are then uploaded to download.xcsoar.org.

Please feel free to add missing data and correct errors by submitting a [pull request](https://help.github.com/en/articles/creating-a-pull-request)! When doing so, please write in the comments what the source of the new data is, so it's easy to verify.

## Relation to [xcsoar-data-repository](https://github.com/XCSoar/xcsoar-data-repository)
There is a sister repository: [xcsoar-data-repository](https://github.com/XCSoar/xcsoar-data-repository) that generates a [repository](http://download.xcsoar.org/repository) file of all the resources available for [xcsoar's](https://xcsoar.org) File Manager. Files here are included, and any changes to file names / paths need to be also changed / added in that repository.