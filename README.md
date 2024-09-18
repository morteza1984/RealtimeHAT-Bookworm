Real-Time HAT™
===


## Clone and install

```
git clone --depth 1 git clone --depth 1 https://github.com/morteza1984/RealtimeHAT-Bookworm-32bit-Beta.git
cd RealtimeHAT
chmod +x install.sh
./install.sh
```
## Copy bitstream

```
Contact InnoRoute to obtain a bitstream for your RT-HAT devices.
Copy the files into /usr/share/InnoRoute 
Reboot your RT-HAT
After login wait up to 1 minut
```

## Testing

```
Connect Port#1 of your Realtime-HAT to the Ethernet port of your PI
Connect Port#0 (RT0) and to a NIC of a PC that has tcpdump or wireshark or similar tools
Both leds of RT0 must be on on now
For sending test frames from RT0 to the PC run:sudo mz RT0 -c10000  -d 20m -A rand  -a rand -b ff:ff:ff:ff:ff:ff  -p 100 "81:00:e0:01:22:f0"



```
