An existing model of Self-resonating
vibrotactile instrument, a string instrument with coupled finite
different schemes have been implemented in Faust and ported
to Max/MSP. Here, gestures recorded from a smartphone and
handled through Open Sound Control have been mapped to
the synthesis’ parameters, using a set of computed mid-level
movement descriptors.


InstallationRequirements

Max/MSP

- Download the odot package .zip file: https://github.com/CNMAT/CNMAT-odot/releases/download/1.3.0/odot-Max-1.3.0.zip
- Open the .zip file and copy the odot folder in your /Max 8/Packages folder.
- Download the modosc package .zip file: https://github.com/motiondescriptors/modosc/archive/main.zip
- Open the .zip file and copy the modosc folder in your /Max 8/Packages folder.
- in Max packages, download and install The HISSTools Impulse Response Toolbox: https://github.com/HISSTools/HISSTools_Impulse_Response_Toolbox



Android smartphone

- Download MultiSense OSC: https://play.google.com/store/apps/details?id=edu.polytechnique.multisense.release&hl=en&gl=US


—————————————————————————————————————————————————————————————————————————


To run the application

- open Triphon.maxpat
- if on Mac, everything should be set (just be sure to use the CoupledBowedPlucked2~.mxo object)
- if on Windows, change the object by renaming it in the main patch (the used object should be CoupledBowedPlucked2~.mxe64)


on your Android device, in the MultiSense OSC app

- set IP address of your PC (both the PC and the smartphone should be connected to the same WiFi network)
- set port 8000
- enable:
- Accelerometer (/multisense/accelerometer/x-y-z)
- Gyroscope (/multisense/gyroscope/x-y-z)
- Orientation (/multisense/orientation/roll-pitch-yaw)

- back in Triphon.maxpat, enable Audio out
- move and play! 

- the application runs also without having the FSR connected to the Arduino Uno, in this case it’s not possible to hold a sustained pitch 
