# PMR446-channels-for-CHIRP
Pre-configured settings for [CHIRP](https://trac.chirp.danplanet.com/chirp_next/next-20230509/) reprogramming tool to tune a Quansheng UV-K5(8) (and similiar) radios into PMR446 frequensies with 5W transmit power.

200 memory slots of the UV-K5(8) are utilized for 8 PMR channels and 24 subchannels. (200 = 8 * (1+24))

## Setting files
The channel settings are in file `pmr_UV-5R.csv`. You can import it in the CHIRP. This is a regular CSV text file, so you can also inspect and edit it in a text editor or in a spreadsheet.

## Subchannels i.e. Tone i.e. CTCSS 
If you are not familiar with PMR, here's some basic information about subchannels. 
Subchannels (e.g. "13" in a channel "3-13") use the same frequency as the main channel (e.g. "3" or "3-0"), but they add an unhearable tone (sine wave), which is makes it possible for the receiving end to filter out other subchannels, and listen only the one that has right tone. This way multiple parties can operate on same frequency simultaneously without hearing each other. If you use the main channel, then you hear every subchannel, but no other subchannel hears you. So, I highly recommended using subchannels.

## Legal
Most baofeng are locked outside PMR446 frequencies, and these CHIRP settings do not unlock the radio. These channels work only with the unlocked radio. Unlocking is probably possible, but it is not covered here. In most european countries it is illegal to transmit on PMR446 frequencies using higher powers than 0.5W. These CHIRP settings are for e.g. Australia and New Zealand where 5W transmit power is allowed. These channel settings can be modified to use 0.5W transmit power by opening the CSV file in a text editor, and searching and replacing all occurences of "5.0W" with "0.5W".


for total of 38 subchannels there are subtones:

1	67.0
2	71.9
3	74.4
4	77.0
5	79.7
6	82.5
7	85.4
8	88.5
9	91.5
10	94.8
11	97.4
12	100.0
13	103.5
14	107.2
15	110.9
16	114.8
17	118.8
18	123.0
19	127.3
20	131.8
21	136.5
22	141.3
23	146.2
24	151.4
25	156.7
26	162.2
27	167.9
28	173.8
29	179.9
30	186.2
31	192.8
32	203.5
33	210.7
34	218.1
35	225.7
36	233.6
37	241.8
38	250.3
