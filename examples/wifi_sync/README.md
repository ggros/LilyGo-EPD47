# How to put some ffat (NO SD)

see https://github.com/marcmerlin/esp32_fatfsimage

## Create fatfs image of data dir

`./fatfsimage -l5 img.ffat 3516 data/`

## flash at right partition position
`esptool.py write_flash 0xc90000 img.ffat`

# Check result in web browser
- go to http://ip-of-device/edit
- then right click on a sample image and select "Display to OSD"