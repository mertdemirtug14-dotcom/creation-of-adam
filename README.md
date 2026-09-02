# Creation of Universe - GRUB Theme

### The Story Behind This

I actually made this GRUB theme just for my own setup at first, but figured I'd share it here in case anyone else likes it.

The whole idea behind this theme is about "beginnings". Since a bootloader is literally what starts up your OS and wakes up your machine, I wanted to capture that exact vibe.

The quote *"From Dust and Spark, We Rise"* is all about how the universe starts from something tiny. Think of the Big Bang—just dust and a single spark, and suddenly everything comes to life. As for the look, the ASCII art takes from Michelangelo's *Creation of Adam*. While the original painting is about Adam coming to life in flesh and blood, this ASCII version represents the exact second your system wakes up. It's there to really nail that feeling of a "first creation" every time you turn on your PC.

**Really mindblowing right? hahaha**

<img alt="Image" src="https://github.com/user-attachments/assets/d04619fc-e6a5-42f0-9318-0d56ea03e940" />

## Installation

1. Clone the repository or download the source code:
   ```bash
   git clone https://github.com/dirgaydtm/creation-of-universe.git
   ```

2. Copy the theme directory to your GRUB themes folder (creating the directory if it doesn't exist):
   ```bash
   sudo mkdir -p /boot/grub/themes
   sudo cp -r creation-of-universe /boot/grub/themes/
   ```

3. Edit your GRUB configuration file:
   ```bash
   sudo nano /etc/default/grub
   ```

4. Add or modify the following line in `/etc/default/grub` to point to the `theme.txt` file:
   ```text
   GRUB_THEME="/boot/grub/themes/creation-of-universe/theme.txt"
   ```

5. Update GRUB to apply the changes:
   - On Debian/Ubuntu-based systems:
     ```bash
     sudo update-grub
     ```
   - On Arch Linux / Manjaro:
     ```bash
     sudo grub-mkconfig -o /boot/grub/grub.cfg
     ```
   - On Fedora/RHEL:
     ```bash
     sudo grub2-mkconfig -o /boot/grub2/grub.cfg
     ```

## Notes

- Make sure you copy the entire folder into your GRUB themes directory, as the `theme.txt` references the background image, fonts, and selection assets in the same directory.
- Just a heads up, this theme is only built for 1920x1080 right now. If you need it in a different size, let me know by opening an issue or feel free to drop a Pull Request!

