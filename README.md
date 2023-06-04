## This guide was written by Ahmad ghoniem

https://www.linkedin.com/in/ahmad-ghoniem/

## Learn How to effortlessly download, convert and split youtube videos using yt-dlp and ffmpeg software


- Steps
1. Extract the Folder
2. open command prompt by typing CMD

![Untitled](https://github.com/ahmadghoniem/yt-dlp-guide/assets/60299751/5bbbe872-4627-4bc9-8a30-5c5e713b57f1)


3. run yt-dlp -U to update yt-dlb to the latest version (make sure it's a capital U and not lowercase u)
4. use one of the following commands

## Single video

1. Downloads video file

   `yt-dlp -S "res:720" -o "%(title)s.%(ext)s" "YOUTUBE_VIDEO_URL"`

2. Converts a single video to Mp3 format by extracting Audio from a video

   `yt-dlp --extract-audio --audio-format mp3 --audio-quality 0 -o "%(title)s.%(ext)s" "YOUTUBE_VIDEO_URL" --ffmpeg-location "ffmpeg\bin"`

## Playlist

1. Download All playlist videos and saves them into a folder named with playlist's title

   `yt-dlp -S "res:720" -o "%(playlist_title)s\%(title)s.%(ext)s" "YOUTUBE_PLAYLIST_URL"`

2. Download playlist videos starting from START to END and saves them into a folder with playlist's title

   `yt-dlp -S "res:720" -I "START:END" -o "%(playlist_title)s\%(title)s.%(ext)s" "YOUTUBE_PLAYLIST_URL"`

3. Download All playlist videos and converts them to Mp3 and saves them into a folder with playlist's title

   `yt-dlp --extract-audio --audio-format mp3 --audio-quality 0 -o "%(playlist_title)s\%(title)s.%(ext)s" "YOUTUBE_PLAYLIST_URL" --ffmpeg-location "ffmpeg\bin"`

4. Download playlist videos from START:END and converts them to Mp3 and saves them into a folder with playlist's title

   `yt-dlp --extract-audio --audio-format mp3 --audio-quality 0 -I "START:END" -o "%(playlist_title)s\%(title)s.%(ext)s" "YOUTUBE_PLAYLIST_URL" --ffmpeg-location "ffmpeg\bin"`

- FYI: you can replace `%(playlist_title)s\%(title)s.%(ext)s` with `%(playlist_title)s\%(playlist_index)%s- (title)s.%(ext)s`
  to save the video with it's index followed by it's name

## Split by Chapters

1. Downloads video file, split it by chapters and saves them to a folder with the video's title

   `yt-dlp -S "res:720" -o "chapter:%(title)s\%(section_number)s - %(section_title)s.%(ext)s" --split-chapters "YOUTUBE_VIDEO_URL" --ffmpeg-location "ffmpeg\bin"`

- FYI:you can replace `"chapter:%(title)s\%(section_number)s - %(section_title)s.%(ext)s"` with `"chapter:%(title)s\%(section_title)s.%(ext)s"`
  to save the video with the chapter name only without the index

# link🔗

### Download ffmpeg and yt-dlp zipped
https://mega.nz/file/0GMA0BYK#97knvxwbYYFz8IrFN60qyKObHfCp5RnLr-DbsPYcjf4

### yt-dlb github repo

https://github.com/yt-dlp/yt-dlp#installation

### yt-dlb download link

https://github.com/yt-dlp/yt-dlp/releases/latest/download/yt-dlp.exe

### ffmpeg website

https://ffmpeg.org

### ffmpeg download link

https://www.gyan.dev/ffmpeg/builds/ffmpeg-git-full.7z
