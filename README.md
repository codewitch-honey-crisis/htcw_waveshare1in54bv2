# Waveshare 1.54 inch (b, version 2) 3-color - waveshare1in54bv2

A GFX enabled device driver for the Waveshare 1.54 inch (b, version 2) 3-color e-paper display

This library allows GFX to bind to a Waveshare 1.54 inch (b, version 2) 3-color display so that you can use it as a draw target.

Documentation for GFX is here: https://www.codeproject.com/Articles/5302085/GFX-Forever-The-Complete-Guide-to-GFX-for-IoT

To use GFX, you need GNU C++14 enabled. You also need to include the requisite library. Your platformio.ini should look something like this:

```
[env:esp32-waveshare2in13b]
platform = espressif32
board = node32s
framework = arduino
lib_deps = 
	codewitch-honey-crisis/htcw_waveshare1in54bv2@^0.9.8
lib_ldf_mode = deep
build_unflags=-std=gnu++11
build_flags=-std=gnu++14
```

Note: Prerelease. Partial update is supported by the display itself but is not working in the driver. When it does end up working it will not require a code change. I may scrap it for this display, because from what I've seen it's not great.