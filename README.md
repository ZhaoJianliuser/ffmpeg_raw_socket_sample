# ffmpeg-socket
利用ffmpeg播放socket接收到的视频文件

运行simplest_ffmpeg_men_player.out

服务器： socket/server

思路：接收到数据放到内存，ffmpeg直接从内存中读取数据，解码播放


# build

# install dependences :
sudo apt-get install -y autoconf automake build-essential git libass-dev libfreetype6-dev libsdl2-dev libtheora-dev libtool libva-dev libvdpau-dev libvorbis-dev libxcb1-dev libxcb-shm0-dev libxcb-xfixes0-dev pkg-config texinfo wget zlib1g-dev

# ffmpeg

sudo apt-get install libavformat-dev
sudo apt-get install libavcodec-dev
sudo apt-get install libswresample-dev
sudo apt-get install libswscale-dev
sudo apt-get install libavutil-dev
sudo apt-get install libsdl1.2-dev

libavformat-dev : 用于各种音视频封装格式的生成和解析，包括获取解码所需信息以生成解码上下文结构和读取音视频帧等功能;
libavcodec-dev : 用于各种类型声音/图像编解码；
libswscale-dev : 用于视频场景比例缩放、色彩映射转换；
libavutil-dev : 包含一些公共的工具函数；

# install ffmpeg
sudo apt-get install ffmpeg