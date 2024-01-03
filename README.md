esp01-m, transceiver, 
never reverse polarity,
always use 3v. if you have any problem it's because your 3v arent stable
connect IO0 to ground while loading code 
board is "Generic esp8266"
115200 baud
when first plugged into power it will go through a "record phase" for 30 seconds, If it reads any NEC (type of IR) signal in that time it will erase all previously stored signals and record all new ones.
the code will store up to 20 signals, when holding a button on a remote for too long it will send multiple signals. use quick presses.
codes get stored after record phase is over
if no new codes are recorded in the "record" phase then it will continue to the "playback phase" after 30 seconds.

possible upgrades, 
-adding a button to enter the record phase so it wont take so long to playback
-versions of the code for other ir signals like Sony or Panasonic, or raw data. (device wont hold that much data)
-some king of led so that we know what phase its in
