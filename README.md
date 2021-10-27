# get_file_from_segments

Downloads and concatenates file segments into a single file in the current
directory

## Requirements

* [wget](https://www.gnu.org/software/wget/)

## Usage

```
$ get_file_from_segments <filename> <file_segment_url> [...]
```

## Example

```
$ get_file_from_segments 'my_file.ts' https://example.com/file-segment-{001-249}.txt

# Output: my_file.txt
```


# get_mp4_from_ts_segments

Downloads, concatenates, and converts telestream (ts) segments into an mp4 file
in the current directory

## Requirements

* [wget](https://www.gnu.org/software/wget/)
* [ffmpeg](https://www.ffmpeg.org/)

## Usage

```
$ get_mp4_from_ts_segments <ts_file> <ts_segment_url> [...]
```

## Example

```
$ get_mp4_from_ts_segments 'my_video.ts' https://example.com/video-segment-{001-249}.ts

# Output: my_video.mp4
```

