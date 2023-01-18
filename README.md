# Video_Carousel
Local video Carousel for firebot

This allows you to play local video files in firebot in a random order with a custom wait duration from a text file. It uses 3 preset effects and is tied into one Event checking for an OBS scene change. If it happens to play through the entire list, it will recreate the original list based on the order it was last played. It will then re-randomize the play list. It will do this indefinitely if allowed to.

# Things to note
 * You must have While loops enabled - You can enable while loops by going to Settings > Advanced > Enable While Loops
 * You must have OBS intergration with FireBot
 * When testing, if you change scenes before the video is done playing, you must wait at least the duration of the video that is currently being played before switching back to the test scene again. If you don't you will cause it to play on top of it self.
 * This is due to the order in which it opperates. It won't trigger the clear overlay effect until the current video is done playing as it is stuck in the wait phase. 

## Install
 To install simply download the Zip and unzip it to your file location 
 
 Import setup for Firebot by going to Settings > Setups > Import Setup
 
 Chose the file "**Clip_Carousel.firebotsetup**" from the location you just unzipped it to, then click Import setup
 
 Fill in the required information
 
 * File location
 * Name of Video list file 1 - be sure to include the file extenstion type
      
      **example_file 1.txt**
      
 * Name of Empty Video list file - be sure to include the file extenstion type
     
     **example_file 2.txt**
     
  * Which scene would you like your videos to play on
