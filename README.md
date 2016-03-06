# bebop-dashboard
#### an OSX application for controlling the Parrot Bebop Drone

####What's working:
* Takeoff, Land (T key, L key)
* Forward, Left, Back, and Right (W A S D keybindings, first-person shooter style)
* Higher, Lower (Up arrow, Down, arrow)
* Rotate left, Rotate right (Left arrow, Right arrow)
* Hover (release the key you're currently pressing)
* GPS: latitude, longitude, altitude update on dashboard

####What we're currently working on:
* live-video stream (so you don't have to look at the drone, just your screen, this is a top priority for beta release).
* start and stop recording video to disk (tested and working, will not be available until how the user interaction is decided)
* taking/saving pictures by using the spacebar (currently throws error).
* overlaying GPS coordinates onto google maps (not quite clear how this will be achieved, as you connect to the drone's wifi network and lose previous wifi connection which is needed for updating the google map)
* letting user select tactile setting, currently at middle (most methods in node-bebop take a speed of 0-100, logic would be simple but no straightforward interface for it (slider maybe?))

####How to use:
1. Turn your Parrot Bebop drone on
2. Connect to it's wifi network
3. Download and cd into directory
4. Install dependencies (via npm install)
5. Open application (via npm start)
6. Check that you're connected ('connected to drone' will appear on left-hand of black rectangle)

Now that you're in control, anytime you press a key it's icon will turn green until the key is release and the drone goes back into hover mode. Try:

* taking off by pressing the letter 'T'. Land by pressing 'L'.
* moving around with the letters: 'W', 'A', 'S', 'D'.
* moving up and down with the up and down arrow keys.
* rotating the drone with the left and right arrow keys.


####Interface

![interface_example](https://github.com/gcwelborn/drone-dashboard/blob/master/drone-dashboard-example.jpg)
