# Learn How to effortlessly download, convert and split youtube videos using yt-dlp and ffmpeg software
### watch video:  https://www.youtube.com/watch?v=Ynyn0HxCEww

## Steps
1. Extract the Folder
2. open command prompt by typing CMD

![Untitled](https://github.com/ahmadghoniem/yt-dlp-guide/assets/60299751/5bbbe872-4627-4bc9-8a30-5c5e713b57f1)

3. run yt-dlp -U to update yt-dlb to the latest version (make sure it's a capital U and not lowercase u)
4. use one of the commands below 

## Single video

1. Downloads video file

   `yt-dlp -S "res:720" -o "%(title)s.%(ext)s" "YOUTUBE_VIDEO_URL"`

2. Converts a single video to Mp3 format by extracting Audio from a video

   `yt-dlp --extract-audio --audio-format mp3 --audio-quality 0 -o "%(title)s.%(ext)s" "YOUTUBE_VIDEO_URL" --ffmpeg-location "ffmpeg\bin"`

## For downloading Multiple videos at once you can save them into a playlist and use the playlist commands

## Playlist

1. Download All playlist videos and save them into a folder named with the playlist's title

   `yt-dlp -S "res:720" -o "%(playlist_title)s\%(title)s.%(ext)s" "YOUTUBE_PLAYLIST_URL"`

2. Download All playlist videos, converts them to Mp3 and save them into a folder with the playlist's title

   `yt-dlp --extract-audio --audio-format mp3 --audio-quality 0 -o "%(playlist_title)s\%(title)s.%(ext)s" "YOUTUBE_PLAYLIST_URL" --ffmpeg-location "ffmpeg\bin"`

3. Download playlist videos starting from START to END and save them into a folder with the playlist's title

   `yt-dlp -S "res:720" -I "START:END" -o "%(playlist_title)s\%(title)s.%(ext)s" "YOUTUBE_PLAYLIST_URL"`

4. Download certain videos from a playlist and save them into a folder with the playlist's title

   `yt-dlp -S "res:720" -I "2,5" -o "%(playlist_title)s\%(title)s.%(ext)s" "YOUTUBE_PLAYLIST_URL"`

5. Download playlist videos from START:END, converts them to Mp3 and save them into a folder with the playlist's title

   `yt-dlp --extract-audio --audio-format mp3 --audio-quality 0 -I "START:END" -o "%(playlist_title)s\%(title)s.%(ext)s" "YOUTUBE_PLAYLIST_URL" --ffmpeg-location "ffmpeg\bin"`

6. Download certain videos from a playlist, them to Mp3 and save them into a folder with the playlist's title

   `yt-dlp --extract-audio --audio-format mp3 --audio-quality 0 "res:144" -I "2,5" -o "%(playlist_title)s\%(title)s.%(ext)s" "YOUTUBE_PLAYLIST_URL" --ffmpeg-location "ffmpeg\bin"`


- FYI: you can replace `%(playlist_title)s\%(title)s.%(ext)s` with `%(playlist_title)s\%(playlist_index)%s- (title)s.%(ext)s`
  to save the video with it's index followed by it's name

## Split by Chapters

1. Downloads video file, split it by chapters and saves them to a folder with the video's title

   `yt-dlp -S "res:720" -o "chapter:%(title)s\%(section_number)s - %(section_title)s.%(ext)s" --split-chapters "YOUTUBE_VIDEO_URL" --ffmpeg-location "ffmpeg\bin"`
2. Downloads video file, convert them to Mp3 and split it by chapters and save them to a folder with the video's title

   `yt-dlp --extract-audio --audio-format mp3 --audio-quality 0 -o "chapter:%(title)s\%(section_number)s - %(section_title)s.%(ext)s" --split-chapters "YOUTUBE_VIDEO_URL" --ffmpeg-location "ffmpeg\bin"`
- FYI: you can replace `"chapter:%(title)s\%(section_number)s - %(section_title)s.%(ext)s"` with `"chapter:%(title)s\%(section_title)s.%(ext)s"`

  to save the video with the chapter name only without the index

## End results 
 
![FxzxtrhWIAILMy9](https://github.com/ahmadghoniem/yt-dlp-guide/assets/60299751/015f0deb-7dbc-4707-9e78-3d87cd60d12d)
![FxzyFKFX0AAQOoP](https://github.com/ahmadghoniem/yt-dlp-guide/assets/60299751/237a15d7-00c1-4e70-9360-f6d4279134e7)


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


