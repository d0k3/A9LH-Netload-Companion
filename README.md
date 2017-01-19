# A9NC - ARM9 Netload Companion
A simple companion app to receive and run ARM9 payloads via CIA & A9LH

To send a file, use:
3dslink -a [IP] [payload name]

3dslink is included in devKitARM and also available [from here](http://davejmurphy.com/3dslink/).

The file will be written to a place of your choice on your SD card. At the moment, most places to choose from are in in the [Luma3DS](https://github.com/AuroraWright/Luma3DS) payloads folder.
__Developers please contact me if you need A9NC to write to a different location__. 

To use the chainloader, you need to move your default payload (usually your CFW) at `/A9NC/payload.bin` and copy the chainloader payload to either `arm9loaderhax_si.bin` or `arm9loaderhax.bin`. Typically, `arm9loaderhax_si.bin` will be the right choice, because screen init is not implemented yet.

Todo for the chainloader:
  * Adding in screen init
  * Confirm compatibility for all CFW (only tested on Luma at the time of writing, it most likely include Reinand and Luma's forks such as Puma)

Requires devKitARM, libctru and zlib to compile. For easy zlib installation [go here](https://github.com/devkitPro/3ds_portlibs).
