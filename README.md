# AHK_MicMute
## An AutoHotKey script to toggle muting your microphone, with a modified SoundDevices.ahk to get more info.

**1.**  To use the script you first should set your mic level to something not 0 or 100, this value needs to stay the same, so I set mine to approximately 98%(actually came out to 97.999969482421875, which is why you need the modified SoundDevices.ahk)

**2.**  Run the SoundDevices.ahk script. This has been modified to show the full 15 digits that AHK stores numeric values as. This helps for comparing the number and for being more exact to what the value is.

**3.** Find the value you set you mic to (technically I think this could work for any sound device, not just mics but for me a global mic mute toggle is more useful).

**4.** Change the value at the start of the Mute 2.0.ahk script: 
```
  ;**SET THIS TO THE SAME VALUE OF THE VOLUME LEVEL OF THE DEVICE YOU WISH TO MUTE**
  MicVolumeGet = 97.999969482421875
 ```
 
 **5.** Run the Mute 2.0.ahk script. If the value was correctly entered it should mute/unmute 
