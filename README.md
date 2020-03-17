# DEFINITION AND HISTORY 

The eTalk, a multimedia editing tool, is the result of collaborative and transdisciplinary work. It is part of a new form of multimodal digital literacy, while respecting the standards of scientific publishing. It is quotable entirely in details through a share button.

The first version of the eTalks code has been developed in 2012-2015 by Frédéric Kaplan and Cyril Bornet (EPFL, CH), and is available on Github: https://github.com/OZWE/etalk

This new version of the code has been developed by Martial Sankar and Claire Clivaz, SIB Swiss Institute of Bioinformatics, 2016-2019.

Clivaz, Claire, Cécile Pache, Marion Rivoal and Martial Sankar, “Multimodal Literacies and Academic Publishing: the eTalks”, Information Services & Use 35/4 (2015), p. 251-258.

Clivaz, Claire, Marion Rivoal and Martial Sankar, “A New Plateform for Editing Digital Multimedia: The eTalks”, in New Avenues for Electronic Publishing in the Age of Infinite Collections and Citizen Science: Scale, Openness and Trust, Birgit Schmidt and Milena Dobreva (eds.), IOS Press, 2015, p. 156-159.


# HOW TO CREATE AN ETALK USING THE CONTAINER 

This etalk setup is suitable for eduction purpose. It permits to use and test the etalk application on the user's own plateform. It uses the docker-compose tool to set-up the application services (etalk php/apache, mysql, phpmyadmin). 


## REQUIREMENTS

- MAC : Requires Apple macOS Yosemite 10.10.3 or above

- WINDOWS : Requires Microsoft Windows 10 Professional or Enterprise 64-bit

- Browsers: Google Chrome; Safari (version ≥7); Internet Explorer (version 11).



## FIRST STEP : INSTALL DOCKER and Run the etalk virtual machine (VM)

1. INSTALL docker (free) for your desktop (windows, osx or linux) https://www.docker.com/products/docker#

2. Download or clone this repository.

3. Open a terminal in linux or open the "docker quick start terminal" in MacOSX and Windows (that comes along with the installation).

4. Go Inside the directory (use `cd /path/to/directory` more info here [:link:]( https://fr.wikipedia.org/wiki/Cd_(commande)) )

5. Secondly, build the image with : 

	```
	$ docker-compose build
	```

6. Then, run the etalk application with :

	```
	$ docker-compose up -d
	```

7. Open a browser

	On linux : 
	go to the url http://localhost:88 for the  __viewer interface__ or http://localhost:88/edit for the __edit interface__

	On MacOSX or Windows :
	go to the url http://192.168.99.100:88 for the __viewer interface__ or http://192.168.99.100:88/edit for the __edit interface__


## SECOND STEP : MAKE YOUR OWN ETALK

To make your own etalk, you can follow the how-to from the etalk _"Make your own etalk"_ accessing http://192.168.99.100:88
 
1. Create and name a folder that will contain the mp3 files inside `etalkapp/etalk-master/data/`

2. go to the __edit interface__  and start editing your etalk.

## License summary

GPULv3 license; complete version: https://github.com/cclivaz/etalk-docker/blob/master/LICENSE.md
Summary: This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

License of the first version 2012-2015: https://github.com/OZWE/etalk/blob/master/LICENSE.md
Copyright (c) 2012-2013 OZWE SàRL: Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
