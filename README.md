# TP-Link-Archer-V3--RTL8812BU-Monitor-mode
Ubunto 20.0 LTS TP-Link-Archer-V3 Driver with monitor mode

Linux anwita-Inspiron-3558 5.13.0-51-generic #58~20.04.1-Ubuntu SMP Tue Jun 14 11:29:12 UTC 2022 x86_64 x86_64 x86_64 GNU/Linux

HOW TO KNOW tp LINK version

command

$ lsusb 

Bus 002 Device 005: ID 2357:0115 TP-Link 802.11ac NIC
# 2357:0115 

Compilation Commands

sudo apt-get update 
sudo apt-get install build-essential dkms

make

sudo make install 

or Manually 
sudo insamod 88x2bu.ko

or 
./deploy.sh

# Monitor Mode

$ sudo airmon-ng check kill -----very important command to gett all capture packets including eapol

$suod iwconfig wlx54af9784dde0 mode monitor  

  wlx54af9784dde0 : 
          
          IEEE 802.11b  ESSID:""  Nickname:"<WIFI@REALTEK>"          
          
          Mode:Monitor  Frequency:2.412 GHz  Access Point: Not-Associated   
          
          Sensitivity:0/0  
          
          Retry:off   RTS thr:off   Fragment thr:off
          
          Power Management:off
          
          Link Quality=0/100  Signal level=-100 dBm  Noise level=0 dBm
          
          Rx invalid nwid:0  Rx invalid crypt:0  Rx invalid frag:0
          
          Tx excessive retries:0  Invalid misc:0   Missed beacon:0







