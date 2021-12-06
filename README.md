# Chromebook 3
All things shiny and chromified for *Samsung Chromebook 3* - *CELES*.

***Note***: 
---
## Baby Steps
  1. Enable Developer Mode
      - press ESC+F3(Refresh)+Power

  2. Boot ChromeOS and open Terminal
      - Press *CTRL+D* at the white "ChromeOS is missing or damaged" (or "OS verification is OFF") screen
      - Configure Wi-Fi and log in (Guest account is fine)
      - press *CTRL+ALT+T* open terminal
      - type *shell* + *enter* key for usable shell

  3. Update firmware
      - Samsung Chromebook 3 - *Intel Braswell* models require firmwre flashing. See [here](https://chrx.org/#chromebooks).
      - Run in ChromeOS:
        ```
         cd; curl -LO mrchromebox.tech/firmware-util.sh
         sudo install -Dt /usr/local/bin -m 755 firmware-util.sh
         sudo firmware-util.sh
        ```
      - Run in linux:
          ```
          cd; curl -LO mrchromebox.tech/firmware-util.sh && sudo bash firmware-util.sh
          ```
          **any issues see [this](https://mrchromebox.tech/#fwscript) page.*
          
---
## Boot Configurations

###### *CHRX* - dual boot Linux & ChromeOS

```code
curl https://chrx.org/ | sudo tar xzfC - /usr/local && chrx
```

- Follow on-screen instructions
- ``` chrx -p {$PKG_NAME}``` installs additional pkg's

---
## Tool Links

1. [Firmware Flash Utility](https://mrchromebox.tech/#fwscript)
3. [CHRX](https://chrx.org/)
