# Notes on Files in Linux📂

## Types of Files
- **Regular files**: Text, images, binaries, etc.
- **Directories**: Folders containing files or other directories.
- **Special files**: Devices, pipes, sockets, etc.

## File Permissions
- **Read (r)**: View file contents.
- **Write (w)**: Modify file contents.
- **Execute (x)**: Run the file as a program.

## Common Commands👨‍💻
- `ls` – List files and directories.
- `cp` – Copy files.
- `mv` – Move or rename files.
- `rm` – Remove files.
- `touch` – Create empty files.
- `cat`, `less`, `more` – View file contents.

## File Paths
- **Absolute path**: Starts from root (`/`), e.g., `/home/user/file.txt`
- **Relative path**: Relative to current directory, e.g., `../file.txt`

## Hidden Files
- Files starting with `.` are hidden (e.g., `.bashrc`).

## Links🔗
- **Hard link**: Another name for a file.
- **Symbolic link (symlink)**: Shortcut to another file.
- create link by:
  ```bash
  ln -s original_path link_name
  ```
- We can access the contents in the original path using link from the directory containing link using the link name easily.
- Remove link:
  ```bash
  unlink link_name
  ```
  rm is also used to remove the link.

## File Ownership
- Each file has an owner and a group.
- Use `chown` to change owner, `chmod` to change permissions.

## Viewing File Details
- `ls -l` – Long listing with permissions, owner, size, and date.
- `stat filename` – Detailed file information.
