ColorImporter
==============

ColorImporter imports your "Font & Colors" settings from Visual Studio to SQL Server Management Studio.


Supported Versions
-----------------------------

Visual Studio : 2005, 2008, 2010
Management Studio : 2005, 2008

Usage
-----------------------------

ColorImporter is a command line utility which takes two arguments. The first one is the source version and the second one the destination version. Both of them are the release year, for example :

     ColorImporter 2010 2005
	 
Will import the color settings from VS 2010 to Management Studio 2005.

If you don't provides the parameters, the defaults are the 2008 versions for both source and destination.


Internals
-----------------------------

The goal is achieved by copying some registry keys from the Visual Studio folder to the Management Studio one.

Acknowledgement
-----------------------------
 
 The code is heavily based on the work of Tomas Restrepo : http://winterdom.com/2007/10/colorschemesinsql2005managementstudio. I only added the possibility the choose the versions to use and did some code cleaning.