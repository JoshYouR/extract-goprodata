## Basic CLI for extracting gpx data from GoPro Videos
### Prerequisites
This CLI uses ffmpeg and ffprobe, which are not included in this package.

You must have ffmpeg and ffprobe installed on your system, and you must set your system `PATH` environment variable to include the
path to the ffmpeg and ffprobe executables.

They can be found on [ffmpeg's downloads page](https://ffmpeg.org/download.html).

### Installation
Install with `npm -i -g extract-goprogpx`.

Global installation is necessary for the CLI to be used in any directory in the terminal.

### Usage
In terminal shell, use `extract-goprogpx -input [path/to/video-name] -output [path/to/file-name]`.

Alternatively, use `-i` instead of `-input`, `-o` instead of `-output`.

> Don't add the file extension to the `-output` name.

If your GPX file contains no points, it is likely that the camera did not have a GPS lock when you started recording.

### Credit
- ffmpeg
- fluent-ffmpeg/node-fluent-ffmpeg
- ffprobe
- ScottyFillups/ffprobe-client
- JuanIrache/gopro-telemetry
- yargs/yargs