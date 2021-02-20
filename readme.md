# Hackintosh-Intel-i5-10600-RX560-AsRock-B460M-Pro4
Big Sur

Catalina is on the catalina branch
# Info PC

```
MB: AsRock B460M Pro4 $110
CPU: Intel® Core™ i5-10600 $265
VGA: Intel UHD Graphics 630 $0
VGA: Sapphire RX560 Pulse OC 2GB Used $65
RAM: 24GB HyperX DDR4 16GB+8GB 3200Mhz@2666MHz FURY Black $120
SSD: Samsung 970 EVO 500GB used $65
Bluetooth: Asus USB-BT400 $10
Case + PSU: Gamemax ET-211-450 450W Black $28
```

# Hackintosh + OpenCore 0.6.6

- https://dortania.github.io/OpenCore-Desktop-Guide

# Works

- Sleep
- Wake
- Audio
- Ethernet
- Bluetooth
- DisplayPort + HDMI simultaneously
- All USB ports (Full 3.0 + 2.0 + type C)
- Both motherboard and rx560 ports simultaneously

# Result

![Info](/images/info.png)
![Info](/images/ssd.png)
![Info](/images/info.jpg)
Geekbench 5 https://browser.geekbench.com/v5/cpu/3174324

Geekbench 5 + AsRock BFB 125W https://browser.geekbench.com/v5/cpu/3180343
https://www.asrock.com/microsite/2020BFB/
https://www.ixbt.com/news/2020/05/17/asrock-bfb-core-i5-9400.html
![Geekbench](/images/gb-BFB125.png)

Cinebench R20 Multi Core
![Cinebench](/images/cb-mc.jpg)

Cinebench R20 Multi Core + AsRock BFB 125W
![Cinebench](/images/cb-AsRockBFB125W.jpg)

Cinebench R20 Single Core
![Cinebench](/images/cb-sc.jpg)

Geekbench 5 iGPU https://browser.geekbench.com/v5/compute/1327011
![Cinebench](/images/gpu_test.png)

# Note

The file config.plist.

Please change MLB, SystemSerialNumber, SystemUUID into your code:

```
<dict>
    <key>AdviseWindows</key>
    <false/>
    <key>MaxBIOSVersion</key>
    <false/>
    <key>MLB</key>
    <string>xxxxxxxxxxxxxxx</string>
    <key>ProcessorType</key>
    <integer>0</integer>
    <key>ROM</key>
    <data>ESIzRFVm</data>
    <key>SpoofVendor</key>
    <true/>
    <key>SystemMemoryStatus</key>
    <string>Auto</string>
    <key>SystemProductName</key>
    <string>iMac20,1</string>
    <key>SystemSerialNumber</key>
    <string>xxxxxxxxxxx</string>
    <key>SystemUUID</key>
    <string>xxxxxxxx-xxxxx-xxxxx-xxxx-xxxxxxxx</string>
</dict>
```
