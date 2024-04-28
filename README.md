**! ! D E P R E C A T E D ! !**

**This code was replaced for the [ESPNowCam Library](https://github.com/hpsaturn/esp32s3-cam)**

---

## ESPNow Camera 

Proof of concept using an ESP32 camera and ESPNow on broadcast mode to have video streaming to others ESP32 using ESPNow.

## Build and Upload

```cpp
git clone --recursive https://github.com/hpsaturn/espnow-camera.git
cd espnow-camera
``` 

We need remove extra target by this [issue](https://github.com/espressif/esp32-camera/issues/454):

```bash
cd lib/esp32-camera
rm -r target/esp32s2 target/esp32s3/
cd ../..
``` 

Build and upload:

```bash
pio run --target upload
``` 

## Update firmware

```cpp
git submodule update --init --recursive
pio run --target clean
pio run --target upload
```
