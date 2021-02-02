# bibabo

ffmpeg -y -i 你的名字.mp4 -vcodec copy -acodec copy -vbsf h264_mp4toannexb 你的名字.ts
ffmpeg -i 你的名字.ts -c copy -map 0 -f segment -segment_list playlist.m3u8 -segment_time 5 你的名字%03d.ts
