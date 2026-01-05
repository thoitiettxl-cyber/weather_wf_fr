# WiFi Country Code FR

Force WiFi country code to France (FR) on Android boot.

## What it does

Automatically executes `cmd wifi force-country-code enabled FR` after your device boots, enabling access to additional WiFi channels (especially 5GHz band).

## Why use this?

- 🚀 **Unlock 5GHz channels:** Access DFS channels (100-140) restricted in some regions
- ⚡ **One-time setup:** No need to manually run commands after every reboot
- 🔧 **Lightweight:** Runs once on boot, no background services

## Requirements

- KernelSU
- Android 16

## Installation

1. Download `weather_wf_fr.zip`
2. Install via KernelSU
3. Reboot

## Verify

```bash
su -c "cmd wifi status | grep -i country"
```

Expected: `Country Code: FR`

## ⚠️ Disclaimer

**USE AT YOUR OWN RISK**

This module modifies system-level WiFi settings. The author assumes **NO responsibility** for:

- ❌ Hardware damage (overheating, component failure)
- ❌ Violation of local wireless regulations
- ❌ Interference with other devices or radar systems
- ❌ Legal consequences in your jurisdiction
- ❌ Loss of WiFi functionality
- ❌ Any other direct or indirect damages

By using this module, you acknowledge that:
- You understand the risks involved
- You are solely responsible for compliance with local laws
- You accept full liability for any consequences
- The author provides this software "AS IS" without warranty of any kind

**If you're unsure about legality in your region, DO NOT USE THIS MODULE.**

## Uninstall

Remove module in Magisk Manager and reboot.

## License

MIT License

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
