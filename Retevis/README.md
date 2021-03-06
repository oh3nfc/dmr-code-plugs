## About the files in this directory

The .rdt file is the normal codeplug which your radio programming software
should be able to read.

The .conf file is a human readable version of the same code plug, which
[dmrconfig](https://github.com/sergev/dmrconfig) is also able to write back
to the radio. The .conf files are distributed here with permission from
Serge Vakulenko KK6ABQ.

## RT3_NOCALL_1234

The FinDMR zone in meant for finding quickly if there is a nearby repeater
somewhere. All Finnish 70 cm digital voice & data repeater channels with 12,5
kHz step are included. The TX talkgroups are 244 and 9, but the contact lists
hear a lot more. Consider this, when using that zone for calling or replying
a call.

Zones two to eight, from Espoo to Kouvola are however programmed so that each
channel has only one talkgroup.

 - Finland (244)
 - Lapland (2449)
 - Local (9)
 - QSY 1 (24401)
 - QSY 2 (24402)
 - Worldwide (91)
 - Europe (92)
 - German (910)
 - English (913)
 - Italy (222)
 - Sweden (240)
 - Germany (262)
 - Nordic (927)
 - UK (235)
 - Estonia (248)
 - Parrot (244997)

Unlike with the FinDMR zone, with those zones if you hear something,
you'll transmit to the same talkgroup.

The ninth Analog zone has five simplex channels and 11 repeaters programmed
into it.

## RT3S_GPS_NOCALL_1234

The basic configuration has been duplicated from the RT3 channel layout, so
it's very similar to it.

 - The FinDMR zone contains all the finnish DMR repeaters, including Oulu and Tervola.
 - The SweDMR zone contains the Seskarö (Seittenkaari in Haparanda municipality) and Kalix (Kainuu) repeaters.
 - The AprsDMR zone contains the position reporting via those repeaters.
 - The Pori zone has only one analog channel programmed into it in order to make the most of the mixed mode repeater in Arctopolis.

In case you've purchased a GPS version of the handheld radio, you might as well want to send
position reports to [aprs.fi](https://aprs.fi/). Should you wish to do that, first
verify that you've [correct settings on selfcare](http://blog.retevis.com/how-to-set-rt3s-aprs/), then go outside,
wait for the proper GPS lock and push the transmit button. Leave the radio into
the channel to automatically retransmit the location.

The position reporting should work both from Finland and Sweden.

If you don't want to send your position, then avoid transmitting or staying in the GPS
channels altogether. And if you absolutely hate the idea, then you might want to consider
changing all the GPS lines in the conf file into receive only channels to
prevent yourself from sending the location data accidentally.
