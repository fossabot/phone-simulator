# phone-simulator

![USSD-Client](https://user-images.githubusercontent.com/1968058/27106859-748da2de-5052-11e7-9496-457587d67445.gif)
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bhttps%3A%2F%2Fgithub.com%2FRestComm%2Fphone-simulator.svg?type=shield)](https://app.fossa.io/projects/git%2Bhttps%3A%2F%2Fgithub.com%2FRestComm%2Fphone-simulator?ref=badge_shield)

This project is to simulate the Mobile Phone to do various demos. For now it will only support USSD Messages. It supports pull and push notification.

*Is work in progress, you are welcome to make this better.

About
========

This is a maven project, it was built using JDK 1.8 and it works with Telscale USSD GW 6.2.1, newer versions of USSD GW should be tested.

The project consist of 3 modules:

map-impl

USSD-Client < This is were the magic happens

simulator-core aka 'core'

*Graphics interface was built using JavaFX

How to run
========

1) You have to modify 'SCTPManagement_sctp.xml' located inside 'TelScale-ussd-6.2.1.257/jboss-5.1.0.GA/server/simulator/data/'

At line 4 replace 'hostAddress' for the IP of the machine running USSD-GW

At line 13 replace 'peerAddress' for the IP of the machine running USSD-Client

2) USSD-Client load it's configuration from 'main_simulator2.xml'

SCTP local host: Is the IP of the machine running USSD-Client

SCTP romete host: Is the IP of the machine running USSD GW

Acknowledgements
========

Thanks to Joram Herrera from Somos Discovery for this great work! :)


## License
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bhttps%3A%2F%2Fgithub.com%2FRestComm%2Fphone-simulator.svg?type=large)](https://app.fossa.io/projects/git%2Bhttps%3A%2F%2Fgithub.com%2FRestComm%2Fphone-simulator?ref=badge_large)