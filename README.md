# [Chromebook](https://www.google.com/chromebook/#:~:text=What%20is%20a%20Chromebook%3F)

A place for all things shiny and chromified.

---

## Baby Steps
  1. Enable Developer Mode
      - Press *```[ESC]+[F3(Refresh)]+[Power]```*

  2. Boot ChromeOS
      - Press *```[CTRL+D]```* at boot time
      - Connect to network and log in
      - Open terminal with *```[CTRL]+[ALT]+[T]```* or for VT2 *```[ Ctrl ]+[ Alt ]+[ → ]```*
      - At ***[CROSH](https://chromium.googlesource.com/chromiumos/platform2/+/master/crosh/README.md)*** prompt type *```shell```* + *```[enter]```* for usable ChromeOS shell.

  3. Update firmware with [Firmware Flash Utility](https://mrchromebox.tech/#fwscript)
      - Intel **Braswell** models require firmwre flashing. See [here](https://chrx.org/#chromebooks).
      - Execute in ChromeOS with user ***chronos***:
        ```
         cd; curl -LO mrchromebox.tech/firmware-util.sh
         sudo install -Dt /usr/local/bin -m 755 firmware-util.sh
         sudo firmware-util.sh
        ```
      - Run in [Linux](https://linux.org):
          ```
          cd; curl -LO mrchromebox.tech/firmware-util.sh && sudo bash firmware-util.sh
          ```
          **any issues see [this](https://mrchromebox.tech/#fwscript) page.*
          
---

## Boot Configurations

  Not to be confuse with ChromeOS's [boot modes](https://chromium.googlesource.com/chromiumos/docs/+/HEAD/developer_mode.md#dev-mode).

### ***[CHRX](https://chrx.org/)*** - dual boot Linux & ChromeOS

  ```code
  curl https://chrx.org/ | sudo tar xzfC - /usr/local && chrx
  ```

  - Follow on-screen instructions
  - *Note*: ``` chrx -p {$PKG_NAME}``` installs additional pkg's

---
#### Resources:
[Chromium OS Docs](https://chromium.googlesource.com/chromiumos/docs/+/HEAD/developer_mode.md#dev-mode)

