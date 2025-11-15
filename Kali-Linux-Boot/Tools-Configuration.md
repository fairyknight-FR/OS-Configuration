# Sublime Text :

- To increase the font size in Sublime Text, you can do it in several ways:

### Using Keyboard Shortcuts
- Press `Ctrl` + `+` (plus key) to increase the font size.
- Press `Ctrl` + `-` (minus key) to decrease the font size.

### Using Menu
- Go to `Preferences` → `Settings`.
- In the right pane (user settings), add or modify the font size setting like this:
  ```
  "font_size": 18
  ```
  Change the number to your preferred size. Save the file and the font size will update immediately.

### Temporary Zoom
- You can also hold `Ctrl` and scroll your mouse wheel up to increase font size quickly.

- These methods work in Sublime Text on all platforms including Kali Linux.
---
# Joplin 
- To proceed with installing Joplin after downloading the Joplin app image (typically a .AppImage file), follow these steps:

### Steps to Run Joplin AppImage on Kali Linux

1. [Joplin](https://joplinapp.org/help/install/)
2. **Make the AppImage executable**
3. Open a terminal and navigate to the directory where the Joplin AppImage is downloaded. Run:
   ```
   chmod +x Joplin-*.AppImage
   ```
   This command makes the file executable.

4. **Run the AppImage**  
   Still in the terminal, execute:
   ```
   ./Joplin-*.AppImage
   ```
   Replace `Joplin-*.AppImage` with the exact filename, or use tab completion to auto-complete the filename.

5. **Optional: Create a desktop shortcut**  
   To create a launcher shortcut for easy access:
   - Create a new file `~/.local/share/applications/joplin.desktop`
   - Add the following content (adjust the path accordingly):
     ```
     [Desktop Entry]
     Name=Joplin
     Exec=/path/to/Joplin-*.AppImage
     Icon=joplin
     Type=Application
     Categories=Utility;Office;
     ```
   - Save the file and refresh your desktop environment to see the new launcher.
   ---
# Telegram-Desktop :
   Here is a step-by-step guide to set up Telegram on your Linux system (using the tar file you downloaded), explained in English:

## Telegram Setup on Linux from tar file

1. **Download tar file:**
   You have already downloaded the Telegram tar archive (usually named something like `telegram.tar.xz`).

2. **Extract the tar file:**
   Open a terminal and navigate to the folder where you downloaded the tar file, then run:
   ```bash
   tar -xf telegram.tar.xz
   ```
   This will extract a folder named `Telegram`.

3. **Run Telegram:**
   Navigate to the extracted folder:
   ```bash
   cd Telegram
   ```
   Then run the Telegram binary:
   ```bash
   ./Telegram
   ```
   Telegram will launch, and you can proceed with the setup.

4. **First-time setup:**
   - Choose your language (English by default).
   - Enter your phone number to register or log in.
   - Enter the verification code sent to your phone.
   - Set up your profile (name, photo, etc.).

5. **Optional - Create desktop shortcut:**
   To make Telegram launchable from your app menu:
   -  Crete a file by `root` user = `nano /usr/share/applications/telegram.desktop`
   
   or

   - Create a file named `telegram.desktop` in `~/.local/share/applications/` with the following content:
     ```
     [Desktop Entry]
     Name=Telegram
     Comment=Telegram Messenger
     Exec=/full/path/to/Telegram/Telegram
     Icon=/full/path/to/Telegram/telegram-icon.png
     Terminal=false
     Type=Application
     Categories=Network;InstantMessaging;
     ```
   - Replace `/full/path/to/Telegram/Telegram` with your actual path.
   - Replace icon path accordingly.
   - Save the file and refresh your desktop environment or log out and back in.

- This will allow you to launch Telegram from your desktop environment easily.
---

# OBS-Studio Install :
```bash
apt install obs-studio
```

---
