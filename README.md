## ESPNow Camera 

Proof of concept using an ESP32 camera and ESPNow on broadcast mode to have video streaming to others ESP32 using ESPNow.

## Build and Upload

```cpp
git clone --recursive https://github.com/hpsaturn/espnow-camera.git
cd espnow-camera
pio run --target upload
``` 

## Update firmware

```cpp
git submodule update --init --recursive
pio run --target clean
pio run --target upload
```
