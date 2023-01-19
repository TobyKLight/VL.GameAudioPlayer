# VL.GameAudioPlayer
High level command based audio player for vvvv Gamma.

Install from nuget... coming soon 

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
* Includes original test media (also released under MIT licence, although if you used it a credit as composer would be appreciated...)  

## Expectations
* Only plays out the default sound device, no ASIO 
* Only plays audio files, no recording or live inputs 
* No realtime effects, beat detection or FFT 
(If you need these functions see [VL.Audio](https://github.com/vvvv/VL.Audio) 
* No multitrack support 
* Not intended for tight sync with video files.  
* Does not support MP3 (due to underlying library limitation) 

## Dependencies 
* Based on [SFML.net](https://github.com/SFML/SFML.Net)
* Which is based on the [original SFML](https://www.sfml-dev.org/)
* Some of the audio functionality of SFML comes from [OpenAL](https://www.openal.org/)

## Status 
* 90% complete and working 
* PlayDialog functionality is there but not tested properly because I didn't have a use case. I can imagine there are needs here eg managing localisation or linking mediakeys to dialog data for subtitle display. If someone has a project with a dialog usecase maybe you could contribute to this? 
* Positioning functionality is just left to right pan, in theory the underlying library supports 3D positioning. Again I didn't have a usecase during development so if you've got one and you would like to contribute please get in touch. 

## Licence 
MIT 

## Special Thanks
All those in the vvvv chat for help with various issues during development. 
 
