# 27" iMac 2017 to 5K Display Conversion

Here are my notes from the conversion process. I wanted to use one cable (USB-C) for everything (camera, speakers, microphone) except ethernet, because I already have a faster wireless connection. Ethernet on USB 2.0 could be 100Mbps maximum. If you want to use it, you can connect USB ethernet card to one of the USB 2.0 ports that are outside of the case. Files for 3D printer are included.


## What is included

- Camera 3840 x 2160 12MP
- Original speakers with custom Crossovers (audio polypropylene capacitor and air-cored inductor)
- Microphone is outside of the case for better sound quality, but still needs app with echo canceling for video calls
- Driver Board R1811 V4 (brain of the display)
- Stock Power Adapter reusing iMac power connector
- Current Board DZ-LP0818 (brightness board)
- Noctua fan in position of Apple logo in the back
- USB 2.0 hub (4 ports) for camera and 3x USB 2.0 ports outside of the case


## What you need

- Patience
- Dremel
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
| 2x JST XH (2.54mm) 2 pin, cable - female (stock FAN & Noctua FAN) ![jst xh](images/JST%20XH%202pin%20kabel.jpg) | https://www.gme.cz/v/1514940/jst-xh-2pin-kabel or local store |
| 1x JST PH (2mm) series 4 pin, cable - female (driver board speakers) ![jst ph](images/JST%20PH%202%20mm%204-Pin%20female.jpg) | http://www.hezkyden.cz/shop/konektory-ph20mm-prumyslova-propojka/ or local store |
| 7642.05.01.9/F cable eyelet M4 for power grounding ![cable eyelet](images/cable%20eyelet%20M4%20for%20power%20grounding.jpg) | https://www.gme.cz/v/1499739/764205019-f-kabelove-ocko-m4 or local store |
| 2W 180 Ohm rezistor to make stock fan quiet ![180 ohm rezistor](images/2W%20180%20Ohm%20rezistor.jpg) | https://www.gme.cz/v/1488150/gym-cym-rmo-180r-2w-5-0411-metal-oxidovy-rezistor or local store |
| MOLEX 43640-0301 Micro-Fit 3.0 female 3mm, 1x3pin, for cable ![molex female](images/Molex%20Micro-Fit%203%20pin.jpg) | https://www.gme.cz/v/1502876/molex-43640-0301-micro-fit-30-vidlice-roztec-3mm-1x3piny-prima-na-kabel or local store |
| MOLEX 43031-0007 male for Molex Micro-Fit ![molex male](images/Molex%20Micro-Fit%20krimpovaci%20kontakt.jpg) | https://www.gme.cz/v/1502732/molex-43031-0007-krimpovaci-kontakt or local store |

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


## What to print on 3D printer
