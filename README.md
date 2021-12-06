# Chromebook 3
#### *All things shiny and chromified* for Samsun Chromebook 3 *CELES*.

***Note** - *Intel Braswell* model requires firmwre flashing. See compat list [here](https://chrx.org/#chromebooks)

## Baby Steps
  1. Enable Developer Mode
      - press ESC+F3(Refresh)+Power

  2. Boot ChromeOS and open Terminal
      - Press *CTRL+D* at the white "ChromeOS is missing or damaged" (or "OS verification is OFF") screen
      - Configure Wi-Fi and log in (Guest account is fine)
      - press *CTRL+ALT+T* open terminal
      - type *shell* + *enter* key for usable shell

  3. Update firmware
      - required for Braswell models
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
          **any issues see link*
## Boot Configurations

  *CHRX* for dualbooting Linux alongside ChromeOS
  ```
  curl https://chrx.org/ | sudo tar xzfC - /usr/local && chrx
  ```
  - Follow on-screen instructions
  - *NOTE*: chrx -p {$PKG_NAME} will install additional packages
  - Example: 
  ``` chrx -p steam ```

  5. Repeat steps 2 and 4 to install and configure your new system

---
## Tools List

1. [Firmware Flash Utility](https://mrchromebox.tech/#fwscript)
3. [CHRX](https://chrx.org/)
