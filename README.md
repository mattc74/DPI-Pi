# DPI-Pi
18Bit DPI &amp; Back Light Driver for Raspi

This is a Small PCB Design aiming at using a parallel RGB 3.5" screen directly from the ras-pi GPIO Pins

The Screen used is: Model No. LQ035NC111 320x240 3.5" and is popular in GameBoy Projects.

The following ammendments will need to be made to /boot/config.txt on the pi:

dtoverlay=dpi18
overscan_left=0
overscan_right=0
overscan_top=0
overscan_bottom=0
enable_dpi_lcd=1
display_default_lcd=1
dpi_group=2
dpi_mode=87

framebuffer_width=320
framebuffer_height=240
display_rotate=2
dpi_output_format=24597 #rgb
hdmi_timings=320 1 20 30 38 240 1 4 3 10 0 0 0 60 0 9600000 1
