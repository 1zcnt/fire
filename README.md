# fire

The Doom PSX fire effect ([explained here](https://fabiensanglard.net/doom_fire_psx/))
as a 512-byte x86 boot sector: real mode, VGA mode 13h (320x200), a linear
congruential RNG and no BIOS calls after the mode switch.

## Build and run

```sh
make          # GNU as + objcopy, produces the raw 512-byte image `fire`
make run      # qemu-system-i386 -hda fire
```
