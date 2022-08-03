# WIFIPO120FWT
Nedis WIFIPO120FWT teardown and flashing OpenBeken (OpenBK7231T)

## WB2S -> BK7231T

Unfortunate it does not support tasmota, cause its not esp8266 based like i assumed

instead its using a WB2S wifi Modul

Unfortunate you have to open and solder uart to flash it, in my case i had to complete desolder the modul + power it seperate to be able to flash it


## Links

https://github.com/openshwprojects/OpenBK7231T

https://fcc.report/FCC-ID/2ANDL-WB2S/4580213.pdf

https://www.reddit.com/r/esp8266/comments/wa4alo/flashing_guides_for_wb2swb3scb2s_fan_tuya/

https://community.home-assistant.io/t/detailed-guide-on-how-to-flash-the-new-tuya-beken-chips-with-openbk7231t/437276

https://github.com/openshwprojects/OpenBK7231T_App/releases


## random notes
'''
git clone https://github.com/openshwprojects/OpenBK7231T
cd OpenBK7231T/
git submodule update --init

flashen unter linux:
https://github.com/OpenBekenIOT/hid_download_py.git

cd hid_download_py/
pip install tqdm
python3 uartprogram /home/xeniter/Desktop/OpenBeken/OpenBK7231T_UA_1.12.4.bin -d /dev/ttyUSB0 -w


UartDownloader....
programm....
Getting Bus...  : |   

did not work, maybe caused modul was still connected to power pcb
'''

## front and back images :

https://user-images.githubusercontent.com/83796711/117463559-7c295b00-af58-11eb-8c40-b6ec35cbeef2.jpeg

https://assets.lcsc.com/images/lcsc/900x900/20210713_TUYA-WB2S-csyd_C2844246_back.jpg



                                              |[    ?k/s]
