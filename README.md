# store_for_test

ffmpeg -rtsp_transport tcp -i rtsp://admin:zz123456@192.168.11.119:554/h264/ch1/main/av_stream  -vcodec copy -acodec copy -f segment -segment_time 1500 -segment_list out.list $(date +%Y-%m-%d-%H-%M-%S)-%03d.ts
