**Read this in other languages: [English](README.md), [中文](README_CN.md).**
# luck_pico_rtsp_retinaface
    Test the usage of luckfox-pico plus for running RKNN inference with retinaface and streaming via RTSP.

# Development Environment
+ luckfox-pico SDK

# Compilation
```
export LUCKFOX_SDK_PATH=<Your Luckfox-pico SDK Path>
mkdir build
cd build
cmake ..
make && make install
```

# Execution
Upload the compiled `luckfox_rtsp_retinaface_demo` to luckfox-pico, navigate to the folder, and run:
```
./luckfox_rtsp_retinaface
```
Open the RTSP stream using VLC via rtsp://172.32.0.93/live/0 (modify the IP address according to your actual situation).

**Note**: Before running, please close the default system rkipc program by executing `RkLunch-stop.sh`.