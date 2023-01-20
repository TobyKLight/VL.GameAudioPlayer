# VL.GameAudioPlayer
High level command based audio player for vvvv Gamma.
Tested with vvvv 2021.4.12 stable.  

Install from nuget
In Gamma go to top left menu>Manage Nugets>Command line and type 
```nuget install VL.GameAudioPlayer```

Video tutorial.... coming soon 


## Features 
* Aims to reduce the complexity of getting audio playback into your app while maintaining good performance.
* Loads and plays media without blocking your main thread 
* Removes headaches of managing player instances and building state machines for straightforward background music tasks. 
* Simple organisation paradigm from video games with three main categories of media: Sound Effects, Music and Dialog
* Supports advanced workflows to simplify collaboration with composers and import from audio software (eg Ableton) 
* Use loops of music and play loops in sequence
* Potentially cross-platform (only tested on Windows so far)  
* Documented through interactive helppatches 
* Extract BPM and Bar information for visualisation 
* Includes original test media (also released under MIT licence, although if you use these in a project a credit as composer would be appreciated...)  

![image](https://user-images.githubusercontent.com/4467208/213531125-c706eafe-1181-4256-9f15-136989c2fbd7.png)

## Expectations
* Only plays out the default sound device, no ASIO 
* Only plays audio files, no recording or live inputs 
* No realtime effects, beat detection or FFT 

(If you need these functions see [VL.Audio](https://github.com/vvvv/VL.Audio) )

* No multitrack support 
* Not intended for tight sync with video files.  
* Does not support MP3 (due to underlying library limitation) 

## Dependencies 
* Based on [SFML.net](https://github.com/SFML/SFML.Net)
* Which is based on the [original SFML](https://www.sfml-dev.org/)
* Some of the audio functionality of SFML comes from [OpenAL](https://www.openal.org/)

## Status 
* 90% complete and working 
* PlayDialog functionality is there but not tested properly because I didn't have a use case. I can imagine there are specific needs for working with lots of dialog (eg managing localisation or linking mediakeys to dialog data for subtitle display). If someone has a project with a dialog usecase maybe you could contribute to this? 
* Positioning functionality is just left to right panning. In theory the underlying library supports 3D positioning. Again I didn't have a usecase during development so if you've got one and you would like to contribute please get in touch. 

## Changelog 
* 1.0.1 improved helppatches, added function for MediaStatus command to continuing following the same player while next media has the same path. 
* 1.0.0 initial release 

## Licence 
MIT 

## Special Thanks
All those in the vvvv chat for help with various issues during development. 
 
