FreePBX Module Name:  	Hotel Style Wakeup Calls  

This is a beta version (2.11.4 betaX)of Wake Up Calls module for FreePBX. This
version has a number of improvements over 2.11.3 and is ready for testing

Install Instructions:

From the Linux CLI, first get red of pre 2.11.3 version:
```
amportal a ma uninstall hotelwakeup
amportal a ma delete hotelwakeup
```

Install the most most recent beta from this repo:
```
cd /var/www/html/admin/modules
git clone https://github.com/lgaetz/Hotel-Style-Wakeup-Calls.git hotelwakeup
chown -R asterisk:asterisk hotelwakeup
```
In FreePBX,go to module admin, locate Wakeup Calls in the list and install like normal. Report bugs here or on the PIAF forum.


Whenever you need it, update your beta install to the most recent version:
```
cd /var/www/html/admin/modules/hotelwakeup
git pull
chown -R asterisk:asterisk .
```

To abandon the beta version and revert to 2.11.3:
```
amportal a ma uninstall hotelwakeup
amportal a ma delete hotelwakeup
```
In FreePBX, Module Admin, click "Check Online" and install Wakeup Calls from the FreePBX servers.

This program is free software; you can redistribute it and/or
modify it under the terms of the GNU General Public License
as published by the Free Software Foundation; either version 2
of the License, or (at your option) any later version.
This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.
