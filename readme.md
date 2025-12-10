# U20CAM-1080PDN:

## Hardware 

For hardware please refer to the user manual

## Software 

For software please refer to below link :

[UVC Camera Software](https://github.com/INNO-MAKER/UVC-Camera-Software)



## FAQ

Q1： Why is the test rate not reaching 30 frames on my computer or device, and the displayed actual frame rate is slightly lower than the real frame rate?

A1:   

(1) **Insufficient USB port bandwidth or power supply**: If the USB port bandwidth or power supply is inadequate, it can affect the device's performance. Plug the camera module directly into the computer's USB port to avoid sharing bandwidth with other devices, or use a USB hub with external power supply. Try plugging into a USB 3.0 port, as these ports typically offer stronger driving capabilities.

(2)**Insufficient CPU/MPU/GPU/RAM performance**: This issue is common with o8lder computers or ARM development boards. Older hardware may struggle to process image data quickly, causing the frame rate to fall short. Consider upgrading the hardware platform or reducing the resolution to alleviate the system's load.

(3)**Driver or testing software issues**: This is less common, but if the first two causes are ruled out and the issue persists, consider updating the UVC drivers or switching to another testing software.



Q2：How can we make the camera simulate nighttime conditions while it is operating in daytime mode?

A1：

Cover the blue photosensitive diode on the board completely — either with two fingers or with black tape — and the camera will switch to night mode.



Q3: How can we achieve a clearer and longer viewing distance at night。

A3：If you would like to see farther and more clearly at night, you can replace the six infrared LEDs on the board. These LEDs operate at an 850 nm wavelength. You may refer to the LED datasheet available in the GitHub link for details and select higher-power LED alternatives.

It is also possible to increase the LED output by adjusting (reducing) the series resistors on the board, but please note that doing so will raise power consumption and may shorten the LEDs’ lifespan.
