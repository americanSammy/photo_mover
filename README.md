# Automated Photo Backup Script for macOS

Welcome to the Automated Photo Backup Script for macOS! This script automates the process of transferring photos from your camera's SD card to your Mac, organizing them by date, and optionally deleting them from the SD card.

## How It Works

It's simple.
When you insert your camera's SD card into your Mac, the AppleScript automatically detects the insertion and organizes the photos into folders based on their creation dates. 
It then prompts you to confirm whether you want to delete the photos from the SD card.
The photos are organized and the memory card is ready to use! Done! 

## Installation Instructions

1. **Download**: [Click here](link_to_download_zip_file) to download the script files.

2. **Extract**: Extract the contents of the downloaded zip file to a location of your choice on your Mac.

3. **Set Up Folder Actions**:
   - Open the "AutoBackupPhotos.scpt" file in the "AppleScript Editor" application.
   - Select "File" > "Save As..." and save the script to `/Library/Scripts/Folder Action Scripts` folder.
   - Once saved, insert your camera's SD card into your Mac.
   - Navigate to the folder representing your SD card in `/Volumes/`.
   - Right-click on the SD card folder and choose "Folder Actions Setup...".
   - In the Folder Actions Setup window, click the "+" button.
   - Select the saved script file (AutoBackupPhotos.scpt) from `/Library/Scripts/Folder Action Scripts`.
   - Click "Attach".
   - Close the Folder Actions Setup window.

4. **Customize Shell Script** (Optional):
   - Open the "backup.sh" file in a text editor.
   - Edit the "backup_folder" variable to specify the path to the folder where you want to store the backed-up photos. Save the changes to the shell script.

5. **Run the Program**:
   - Insert your camera's SD card into your Mac.
   - The script will automatically detect the insertion, organize the photos into folders based on their creation dates, and prompt you to confirm the deletion of photos from the SD card.
   - Follow the on-screen prompts to confirm or cancel the deletion process.

## Support and Feedback

If you encounter any issues or have questions about the script, feel free to open an issue [here](link_to_issue_tracker). Your feedback is valuable and helps us improve the script for everyone.

## Enjoy Peace of Mind

With the Automated Photo Backup Script for macOS, you can rest assured that your precious memories are safely backed up and organized on your Mac.

---

TO DO: the script isn't recognizing the memory card from being inserted. It currently works if you run the bash script in the Terminal if you're in the directory where the file is stored. Use the command ./photo_backup.sh
