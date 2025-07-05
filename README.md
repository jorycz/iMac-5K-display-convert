# 27" iMac 2017 to 5K Display Conversion

Here are my notes from the conversion process. I wanted to use one cable (USB-C) for everything (camera, speakers, microphone) except ethernet, because I already have a faster wireless connection. Ethernet on USB 2.0 could be 100Mbps maximum. If you want to use it, you can connect USB ethernet card to one of the USB 2.0 ports that are outside of the case. Files for 3D printer are included.


## What is inside the iMac case

- Camera 3840 x 2160 12MP
- Original speakers with custom Crossovers (audio polypropylene capacitor and air-cored inductor)
- Driver Board R1811 V4 (brain of the display)
- Stock Power Adapter reusing iMac power connector
- Current Board DZ-LP0818 (brightness board)
- Noctua fan in position of Apple logo in the back
- USB 2.0 hub (4 ports) for camera and 3x USB 2.0 ports outside of the case
- Microphone is finally **outside of the case** for better sound quality, but still needs app with echo canceling for video calls
  - I tried microphones inside the case, but my voice was somehow distorted during video calls

## What you need

- Patience
- Prudence
- Dremel or similar tool
- Basic soldering skills with soldering stuff
- Wires for connecting speakers and crossovers with driver board and also modifying the stock fan for quietter operation


## What to buy

### Basics

| Item | URL |
| --- | --- |
| DIY 5K Universal R1811 V.4 Driver Board USB-C Freesync EDP DP1.4 Compatible for iMac LM270QQ1 LM270QQ2 Screen External Monitor - **model LM270QQ1** ![driver board](images/5K%20Display%20Driver%20Board.png) | https://www.aliexpress.com/item/1005002734914614.html |
| High-quality DIY Universal Driver Board 50W Current Board DZ-LP0818 Resolve the Panel brightness problem LM270QQ1 LM270QQ2 - **model LM270QQ1** ![current board](images/Current%20Board%20for%20correct%20brithness.png) | https://www.aliexpress.com/item/1005001660237411.html |
| 4K 3840 x 2160 12MP HD IMX258 USB Camera Module AF/FF 75/80/120/135 Degree 30FPS for Face Recognition - **model 75deg AF** ![camera](images/4k%20USB%20camera.png) | https://www.aliexpress.com/item/1005007360663282.html |
| Noctua NF-A4x10 40mm Computer Case Fan 5V/12V PWM SSO Magnetically Stabilized Bearing Quiet Cooling Fan - **model 12V 4PIN PWM, Other, NO RGB** ![noctua fan](images/Noctua%20Fan.png) | https://www.aliexpress.com/item/1005005402810322.html or local store |
| W1209 DC 12V Heat Cool Digital Thermostat Temperature Controller Miniature Thermostat Temperature Control Switch Panel - **model red** ![W1209](images/W1209%20Digital%20Thermostat%20Control%20Switch.png) | https://www.aliexpress.com/item/1005007254239187.html or local store |
| W1209 DC12V cool temp thermostat temperature control switch temperature controller Acrylic case transparentBox - **model Black** ![W1209 box](images/W1209%20Case.png) | https://www.aliexpress.com/item/1005002657916334.html |
| Single 12V 0.8A DC PWM 2-3 Wire Fan Temperature Control Speed Controller Chassis Computer Noise Reduction Module NTC B 50K 3950 - **model PWM 4Wire** ![PWM reduction module](images/PWM%204%20Wire%20Control%20module.png) | https://www.aliexpress.com/item/1005007103040202.html |
| Small 2.0 USB Hub with 4 ports. I used Vention 4-Port USB 2.0 Hub with Power Supply 0.15m Black ![USB 2.0 hub](images/VENTb8.jpg) | https://www.alza.cz/vention-4-port-usb-2-0-hub-with-power-supply-0-15m-black-d5859680.htm or local store |
| 90 Degree Right Angle USB 3.1 Type C Male To Female Converter USB-C Adapter for Samsung Huawei Smart Phone Portable Connector - **model NO.1** ![usb-c 90 Degree Right Angle](images/90%20Degree%20Right%20Angle%20USB%203.1%20Type%20C%20Male%20To%20Female%20Converter%20USB-C%20Adapter.png) | https://www.aliexpress.com/item/1005004418858018.html |
| LCD Display Screen Adhesive Strip Sticker Tape + Opening Tool Kit for Apple iMac 21.5" A1418 A2116 27" A1419 A2115 - model **model 27inch Adhesive Tool** ![Opening Tool Kit](images/Tool%20Kit%20and%20Adhesive%20iMac%2027%202017.png) | https://www.aliexpress.com/item/1005004826457033.html |
| 1x JST XH (2.54mm) 2 pin, cable - female (stock FAN & Noctua FAN) ![jst xh](images/JST%20XH%202pin%20kabel.jpg) | https://www.gme.cz/v/1514940/jst-xh-2pin-kabel or local store |
| 1x JST PH (2mm) series 4 pin, cable - female (driver board speakers) ![jst ph](images/JST%20PH%202%20mm%204-Pin%20female.jpg) | http://www.hezkyden.cz/shop/konektory-ph20mm-prumyslova-propojka/ or local store |
| 1x JST PH (2mm) series 2 pin, cable - female (power for PWM control board for Noctua fan from driver board) ![jst ph2](images/JST%20PH%202%20mm%202-Pin%20female.jpg) | http://www.hezkyden.cz/shop/konektory-ph20mm-prumyslova-propojka/ or local store |
| 7642.05.01.9/F cable eyelet M4 for power grounding ![cable eyelet](images/cable%20eyelet%20M4%20for%20power%20grounding.jpg) | https://www.gme.cz/v/1499739/764205019-f-kabelove-ocko-m4 or local store |
| 2W 180 Ohm rezistor to make stock fan quiet ![180 ohm rezistor](images/2W%20180%20Ohm%20rezistor.jpg) | https://www.gme.cz/v/1488150/gym-cym-rmo-180r-2w-5-0411-metal-oxidovy-rezistor or local store |
| MOLEX 43640-0301 Micro-Fit 3.0 female 3mm, 1x3pin, for cable ![molex female](images/Molex%20Micro-Fit%203%20pin.jpg) | https://www.gme.cz/v/1502876/molex-43640-0301-micro-fit-30-vidlice-roztec-3mm-1x3piny-prima-na-kabel or local store |
| MOLEX 43031-0007 male for Molex Micro-Fit ![molex male](images/Molex%20Micro-Fit%20krimpovaci%20kontakt.jpg) | https://www.gme.cz/v/1502732/molex-43031-0007-krimpovaci-kontakt or local store |
| Tape 300 x 3,6 mm 100 pcs white ![vorel tape](images/VOREL%20Tape%20300.jpg) | https://www.alza.cz/EN/vorel-tape-300-x-3-6-mm-100-pcs-white-d8069517.htm or local store |
| M3 Screw Bolt Nuts Kit 3x12mm ![m3](images/M3%20sroub%20matka.jpg) | https://www.gme.cz/v/1511744/wurth-slkm3x10-ocelovy-sroub-m3x10mm-phillips-zapustna-hlava-pozinkovany and https://www.gme.cz/v/1511808/wurth-skm3k-matice-m3 or local store |

### Microphone

| Item | URL |
| --- | --- |
| UGREEN Sound Card USB Audio Interface External 3.5mm Microphone Audio Adapter Soundcard for PC Laptop PS4 Headset USB Sound Card - **model 2Ports 15cm** ![sound card](images/USB%20sound%20card%20for%20Microphone.png) | https://www.aliexpress.com/item/1005006519284690.html |
| 2x ADMP401 ADMP404 MEMS Microphone Breakout Module Board For Arduino Universal 1.3cm*1cm 1.5 to 3.3VDC With Pins - **model ADMP404** ![microphones](images/MEMS%20microphones%202x.png) | https://www.aliexpress.com/item/1005005316748856.html |
| 0.1uF Capacitor for MEMS Microphones (1pcs) 直插铝电解电容0.1UF 0.22UF 0.33UF 0.47UF 50V 511MM ±20% Variant: 0.1UF 50V 511 50只 - **model 0.1µF** ![0.1uF capacitor](images/Capacitor%200.1uF%20for%20Microphone.png) | https://www.aliexpress.com/item/1005003133078519.html |

### Crossovers

| Item | URL |
| --- | --- |
| 2x audio polypropylene capacitor 10µF | local store |
| 2x air-cored inductor 0,15mH | local store |

If you don't want to use crossovers, you can connect the speakers to series.


## What to print on 3D printer

All STL files are in stl folder.

- Current Board
- Custom Crossover Left
- Custom Crossover Right
- Driver Board pad 6 mm (for top right side of the driver board)
- Driver Board pad 9 mm (for top left side of the driver board)
- Driver Board
- Microphone Box - front
- Microphone Box - main
- PWM Control Module Box - back
- PWM Control Module Box - main
- R1811 Control Strip - back
- R1811 Control Strip - main
- USB Camera Mount
  - For camera, I used Camera Mount from here https://www.printables.com/model/311111-apple-imac-27-2014-5k-monitor-conversion


## Build

- For disassembly, see any video for example this one from [How-FixIT](https://www.youtube.com/watch?v=96MiQn645jI)
- **Beware!** Use designated opening tool only, otherwise you can cut the cable to display which is near the top. If you use any other cutter, **do not cut too deep!** If do so, you will probably break the ribbon cable and result could be like in this post on Mac Rumors forum [DIY 5k Monitor - success :-)](https://forums.macrumors.com/threads/diy-5k-monitor-success.2253100/post-32835650)
- If you have other model than iMac 2017, check display type before ordering driver board. When you dismount the display, type is in lower right part of the display. For iMac 2017, it is LM270QQ1
- If you don't want to use crossovers, connect the speakers directly to the driver board. Speakers can be connected to series in speaker connector like this ![speaker to series](cimages/800_sound%20speaker%20to%20series.jpeg)

### First cut :)

![first cut](cimages/800_0%20first%20cut-2.jpeg)

### Connecting and first testing

When all parts arrives, test driver board and current board. Pay attention to details. Cables must be positioned exactly as on pictures.

| Brightness cable connection to display | LVDS cable connection to display |
| --- | --- |
| ![bcable](cimages/800_cable%20display%20backlight.jpeg) | ![lvds](cimages/800_cable%20display%20connection%20-%20to%20lcd.jpeg) |


Connect cables to boards. Do not forget R1811 control strip which is on the bottom right corner of driver board on this picture.  
  
![borads test](cimages/1200_boards%20first%20testing.jpeg)

- When you connect power, OSD should appear on display. If not, turn on driver board by button next to remote diode on control strip. Then connect Mac using USB-C port and it should detect display and show desktop. Mine is detected as iMacPro5K.

### Speaker connectors

| Speaker connector with contacts facing you | Description of PINs |
| --- | --- |
| ![speaker connector](cimages/800_sound%20repro%20connection.jpeg) | **Woofer +**<br>**Woofer -**<br>ID link (ignore)<br>ID link (ignore)<br>**Tweeter +**<br>**Tweeter -** |

### Crossovers

**Capacitors** are always connected to **Tweeter +** and **Driver Board +** for every channel  
**Air-cored inductor** are always connected to **Woofer +** and **Driver Board +** for every channel  
**-** are connected together in speaker connector and connected to **Driver Board -** for every channel  

| Crossover testing | PaulD-UK schema from Mac Rumors forum |
| --- | --- |
| ![crossover testing](cimages/800_crossover.jpeg) | ![crossover schema](cimages/crossover%20connection%20PaulD-UK.jpg) |

### Driver Board speaker connection

| Driver Board Audio Connector | Description of channels |
| --- | --- |
| ![driver board audio](cimages/800_driver%20board%20audio%20connector.jpg) | **Left +**<br>**Left -**<br>**Right -**<br>**Right +** |

### Camera

Camera is connected by (included) USB cable to USB 2.0 hub. 3D printed part is a little bigger. I put the camera to lower right corner and I don't have issues with AF or image so I kept it like this.  

![camera](cimages/800_camera%20close.jpeg)

### Power

I wanted to reuse power connector of iMac 2017. If you don't want to, you can skip this section. Otherwise, beware live wire and focus on soldering here.

| Apple Power Connector with Live wire | Soldered Power Connector |
| --- | --- |
| ![apple power connector](cimages/800_power%20conn%20live%20wire.jpeg) | ![soldered power connector](cimages/800_power%20conn%20finished.jpeg) |

| Final connection to stock power adapter | Soldering of Live wire example |
| --- | --- |
| ![final connection](cimages/800_power%20230V%20connection.jpeg) | ![soldering live wire](cimages/800_power%20solder.jpeg) |

### Fans

Power Supply is in iMac case so I need some fresh air in there but also keep display quiet. So I modified Apple logo and placed Noctua fan there which (after small cutout on the left side) fits this space perfectly.

- Use heatgun for a couple of seconds to get rid of the thin cover
- Cut like about 1mm of logo on the left side so fan fits perfectly inside the logo
- Mark 4 holes for mounting the fan
- Then I used thin and very sharp knife to mark circle around fan so I know where to cut the circle to logo

![noctua 1](cimages/1200_fan%20top%20Noctua%201.jpeg)  
![noctua 2](cimages/1200_fan%20top%20Noctua%202.jpeg)  
![noctua 3](cimages/1200_fan%20top%20Noctua%203.jpeg)  
![noctua 4](cimages/1200_fan%20top%20Noctua%204.jpeg)  
![noctua 5](cimages/1200_fan%20top%20Noctua%205.jpeg)  

- Connect fan to extension cable included in Noctua box with fan and then to PWM control module.

![noctua extension](cimages/800_fan%20top%20Noctua%20with%20extension%20cable.jpeg)

- I placed probe of the module behind power supply (top part) so I can check highest temperature area of the display.

![top probe](cimages/800_fan%20top%20Noctua%20probe%20place%20power.jpeg)

- Remove the arrows from JST PH 2 pin connector so it can be connected to driver board.

![jst xh fan noctua](cimages/800_fan%20top%20Noctua%20connector%20removed%20lines.jpeg)

- Connect this connector (later) to driver board here. **Ignore cable colors on my pictures, just connect + on driver board to + cable on PWM module** and the same with -
- Polarity is written on the back of the driver board but to be sure, **use multimeter to check polarity!**

| Power for PWM control module for Noctua fan | Polarity. Check with multimeter! |
| --- | --- |
| ![jst xh noctua control connected to driver board](cimages/800_fan%20top%20Noctua%20power%20connection.jpeg) | - - + + + |

- PWM control module. Connect Noctua extension cable on the right side.

![PWM control module](cimages/800_PWM%20control%20module%20schema.png)

- Solder connectors for power of the PWM module and connect it like this
  - On the right side, there is fully connected PWM control module with Noctua extended cable, power from driver board and (included) probe.
  - On the left side, there is simple relay W1209 module with 180 Ω resistor (hidden in insulation) on +ve wire of stock fan.

![pwm power wires](cimages/1200_fan%20connection%20controllers%20on%20board.jpeg)

