# Demo
![demo.gif](docs%2Fimages%2Fdemo.gif)

# Usage
> ⚠️ FTP download from the bambu printer is very slow, please be patient. 🙂 
> 
> A 10mb file took ~1-2 minutes, but maybe my printer just have not the best wifi signal..

## run with default parameters
bambu_timelapse_download.exe --ip 192.168.0.20 --pass 12345678

## save timelapse file in diffrent directory
bambu_timelapse_download.exe --ip 192.168.0.20 --pass 12345678 --download_dir "C:\Video\3D Druck\Timelapse"

## save timelapse file in diffrent directory & delete timelapse files from ftp after download
bambu_timelapse_download.exe --ip 192.168.0.20 --pass 12345678 --download_dir "C:\Video\3D Druck\Timelapse" -d

# Parameter
| Name                 | Description                           | Required | Default   |
|----------------------|---------------------------------------|----------|-----------|
| ip                   | IP address of printer.                | Yes      | -         |
| port                 | FTP Port.                             | No       | 990       |
| user                 | FTP User.                             | No       | bblp      |
| password             | Access code shown on printer display. | Yes      | -         |
| download_dir         | Download foldername.                  | No       | timelapse |
| ftp_timelapse_folder | FTP timelapse folder on ftp.          | No       | timelapse |
| -d                   | Delete timelapse file after download. | No       | -         |
| -v                   | Show Version                          | No       | -         |