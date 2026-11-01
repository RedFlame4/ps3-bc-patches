# ps3-bc-patches
IPS patch for the PS2 Emulator on full PS2 hardware PS3 models (CECHA/CECHB) to give the cleanest possible video output.

This only impacts video output when the PS2 upscaling option is off and should only be used in combination with an external upscaler.

The current list of changes is as follows:

1. Direct 480i/576i output over HDMI, this does not reduce latency and is solely to allow for external deinterlacing.
2. PAL 576i games no longer receive an erroneous 0.35% scale on the vertical axis.
3. Disabled deinterlacing blur on 480p/576p output, this may make deinterlacing artifacts more apparent but removes vertical blurring.
4. 240p is cleanly linedoubled to 480p, removing the existing vertical blur and unnecessary deinterlacing artifacts.
5. Aspect ratio correction is disabled to avoid horizontal blurring, the aspect ratio will therefore need to be corrected using an external upscaler.