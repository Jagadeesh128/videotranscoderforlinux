# Video Transcoder Script

This script allows for the transcoding of multiple video files into ProRes format, providing users with an efficient way to manage their video files. The script also extracts essential metadata from each input video file.

## Features

- **Batch Transcoding**: Supports transcoding multiple video files in one command.
- **Metadata Display**: Shows key details of the input video files.
- **Automatic Directory Creation**: Creates the output directory if it doesn’t already exist.
- **Graceful Interruption Handling**: Captures SIGINT (Ctrl+C) to exit the script smoothly.

## Requirements

- **FFmpeg**: The script requires FFmpeg and FFprobe. You can install them via your package manager or download them from [FFmpeg's official website](https://ffmpeg.org/download.html).

## Usage

```bash
./transv inputfile1 [inputfile2 ... inputfileN] outputfolder
```

## Arguments

- **inputfile1, inputfile2, ..., inputfileN**: The video files you wish to transcode.
- **outputfolder**: The directory where the transcoded files will be saved.

## Example

```bash
./transv video1.mp4 video2.mp4 /path/to/output
```
## How It Works

- The script checks for a minimum of two arguments (input files and output directory).
- It attempts to create the output directory if it does not exist.
- For each input file:
  - Metadata is extracted and displayed.
  - The video is transcoded to ProRes format.
  - The script confirms successful transcoding for each file.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Contributing

Feel free to fork the repository and submit pull requests for any changes or improvements.

---

This markdown format is suitable for a `README.md` file in your repository.
