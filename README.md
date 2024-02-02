### Bash Script for Managing a Recycle Bin

This bash script provides functionality to manage a recycle bin for files. It allows users to move files to the recycle bin, restore files from the bin, permanently remove files from the bin, and schedule automatic removal of files after a specified time limit.

### Usage

```
Usage: recycle_bin.sh [remv | restore | remvp | schedule_removal] [filename(s)]
```

#### Commands:

1. `remv`: Move files to the recycle bin.
2. `restore`: Restore files from the recycle bin.
3. `remvp`: Permanently remove files from the recycle bin.
4. `schedule_removal`: Schedule automatic removal of files from the recycle bin after a specified time limit.

### Instructions

1. **Setup**: The script will create a directory named `bin` in the user's home directory (`$HOME/bin`) if it doesn't already exist. This directory will be used as the recycle bin.

2. **Functions**:
    - `remv`: Moves specified files to the recycle bin.
    - `restore`: Restores specified files from the recycle bin to their original locations.
    - `remvp`: Permanently removes specified files from the recycle bin.
    - `schedule_removal`: Schedules the automatic removal of specified files from the recycle bin after a specified time limit.

3. **Usage**:
    - Run the script with appropriate commands and filenames to perform desired operations.

### Example Usages:

- Move a file to the recycle bin:
  ```
  ./recycle_bin.sh remv file.txt
  ```

- Restore a file from the recycle bin:
  ```
  ./recycle_bin.sh restore file.txt
  ```

- Permanently remove a file from the recycle bin:
  ```
  ./recycle_bin.sh remvp file.txt
  ```

- Schedule removal of a file from the recycle bin after 10 seconds:
  ```
  ./recycle_bin.sh schedule_removal 10 file.txt
  ```


