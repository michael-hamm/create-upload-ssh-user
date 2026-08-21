upload.sh
Creates a chroot-restricted SFTP/SCP upload-only user.

Usage:
  sudo ./upload.sh USERNAME PUBLIC_KEY_FILE

Example:
  sudo ./upload.sh customer01 ./customer01_ed25519.pub

Upload:
  scp file.zip customer01@server.example:/incoming/

or:
  sftp customer01@server.example
  put file.zip /incoming/file.zip
