WSJF_Grid
=========================

## Overview
Weighted Shortest Job First Grid
This app displays a grid that shows the values used to calculate the WSJF score, 
and then calculate the score. The values in the grid are editable, but the score is not as it is 
calculated based on the values. The columns are sortable, so for example if you want to sort by Score, just
click on the "Score" column.


The Details:
The app is designed to work with Portfolio Items of type "Feature". No other filtering is handled,
but could be added.
The WSJF score calculation is ( Time Value + OERR + User Value)/ Job Size (rounded to nearest integer)
The app assumes Portfolio Items include the following custom integer fields. Make sure the following names are
entered into the Display Name of the integer field. If you change the display name to something else,
be sure to update the app accordingly.

Caveat:
The App.html file has an altered script tag, so if you regenerate the html file you will likely need to hand-modfy
the script tag. Change the src parameter so: src="/apps/2.0p5/sdk.js?wsapiVersion=1.43"

The wsapi version is included to allow access to new methods. Using sdk 2.0rc1 breaks cell editing, so until I
figure that one out this is the workaround.

Time Value <br>
OERR <br>
User Value <br>
Job Size <br>
Score <br>

Screencast Demo
---------------

http://screencast.com/t/aCOOhkpeHdXA

Screenshot
----------

https://github.com/sficarrotta/WSJF_Grid/raw/master/deploy/WSJF_Grid.png

## License

AppTemplate is released under the MIT license.  See the file [LICENSE](https://raw.github.com/RallyApps/AppTemplate/master/LICENSE) for the full text.
