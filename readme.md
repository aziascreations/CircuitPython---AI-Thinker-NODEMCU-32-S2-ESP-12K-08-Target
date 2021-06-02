# 🐍 CircuitPython - AI-Thinker NODEMCU-32-S2 ESP-12K 08 Target

This repository contains the build target for CircuitPython and a AI-Thinker NODEMCU-32-S2 devboard that has an ESP-12K 08 on it.

It also provides the "aesio" module that is usually not present on ESP32-S2 ports even if it works perfectly.

## Board
<table><tr><td>
<img src="https://i.imgur.com/hlmAe4x.png" alt="Picture of the front of the devboard" width="100%">
</td><td>
<img src="https://i.imgur.com/iB3kwzV.png" alt="Picture of the back of the devboard" width="100%">
</td></tr><tr>
<td colspan=2>
<img src="https://i.imgur.com/u3dnwOH.png" alt="Pinout of the devboard" width="100%">
</td>
</tr></table>

## Cloning

### At the root of the repository
```bash
???
```

### In the ports/esp32s2 folder
```bash
git clone x boards/aithinker-nodemcu-32-s2-esp12k-08
```

## Building
```bash
make BOARD=aithinker-nodemcu-32-s2-esp12k-08
```

## Flashing
Use the standard procedure with `0x0000` as the offset for `firmware.bin`.

## Connecting to the USB OTG port
Use the 5V, GND pins near the onboard USB connector and the 2 pins above the GND pin for the D+ and D- wires.

## Known Issues
* The neopixel module and LED references still exist (I don't know how to safely get rid of them)
* The USB PID may cause problems, I don't know how Adafruit and the CircuitPython community chooses them.

## Disclaimer

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
