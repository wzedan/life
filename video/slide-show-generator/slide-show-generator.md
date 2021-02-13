# Don't use online videos generator - SCAM , Slow and useless !!!

## Prerequistes
1. (sudo) gem install fastimage -v 1.8.1

## Usage

1. Add your images in alphabetical order (_note 2 is alphabetically before 11_) in one folder
2. Just run the following pointing to the parent folder in which the images are located. By default it will list all the images with .jpg extension there.

```bash
./ss-generator.rb <input-folder> <output-folder>/<video-name>.mp4
```
**Only Supports MP4 codec**

```bash
./ss-generator.rb --help
Usage: ./ss-generator.rb [options] <input_folder> output.mp4
    -h, --help                       Prints this help
        --size=[WIDTHxHEIGHT]        Output width (default: 1280x800)
        --slide-duration=[DURATION]  Slide duration (seconds) (default: 4)
        --fade-duration=[DURATION]   Slide duration (seconds) (default: 1)
        --fps=[FPS]                  Output framerate (frames per second) (default: 60)
        --zoom-direction=[DIRECTION] Zoom direction (default: random)
        --zoom-rate=[RATE]           Zoom rate (default: 0.1)
        --scale-mode=[SCALE_MODE]    Scale mode (pad, crop_center, pan) (default: auto)
        --dump-filter-graph          Dump filter graph to '<OUTPUT>.filtergraph.png' for debugging
        --loopable                   Create loopable video
        --audio=[FILE]               Use FILE as audio track
        --extension                  images extensions (default: jpg)
    -y                               Overwrite output file without asking
```
## References

1. Almost all code was copied from https://github.com/remko/kburns 
2. https://trac.ffmpeg.org/wiki/Slideshow
3. 