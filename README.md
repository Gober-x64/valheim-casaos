# Valheim CasaOS

This repository helps you run a Valheim server on CasaOS.

The recommended YAML configuration, `Valheim-server_mbround.yaml`, is based on the repository [mbround18/valheim-docker](https://github.com/mbround18/valheim-docker).  
Inspiration was also taken from this [Reddit post](https://www.reddit.com/r/valheim/comments/1bijg8x/valheim_in_casaos/).

## Installation Guide

1. **Download or Copy the YAML Configuration File**  
   Download or copy the content of this [YAML configuration file](https://github.com/Gober-x64/valheim-casaos/blob/main/Valheim-server_mbround.yaml).

2. **Install on CasaOS**  
   - Press the "+" sign and click on "Install a customized app":  
<div align="left">
<img src="https://raw.githubusercontent.com/Gober-x64/valheim-casaos/main/images/Step_1.png" alt="Step 1">
</div>

   - In the new window, click on the import symbol in the upper right corner, next to the "X" symbol:  
<div align="left">
<img src="https://raw.githubusercontent.com/Gober-x64/valheim-casaos/main/images/Step_2.png" alt="Step 2">
</div>

   - In the import window, drag and drop the downloaded file into the upload section in the lower half of the window, or copy the content of the `.yaml` file into the text box above. Press the submit button:  
<div align="left">
<img src="https://raw.githubusercontent.com/Gober-x64/valheim-casaos/main/images/Step_3.png" alt="Step 3">
</div>

3. **Change the Following Environment Variables**  
<div align="left">
<img src="https://raw.githubusercontent.com/Gober-x64/valheim-casaos/main/images/Change_This.png" alt="Change this">
</div>

   **NOTE:**  
   - The password needs to be at least 5 characters long; otherwise, the server won't start.
   - Change the `TZ` variable (Time Zone) depending on your location.

   **OPTIONAL:**  
   - Adjust the memory to your desired size.
   - You may want to change the host-sided volumes to another path (don't change the container volumes).

## Explaining the Default Configuration

The standard configuration includes an auto-backup feature that creates a backup of the world every 15 minutes. After 3 days, old backup files are automatically deleted. There's also an auto-update option enabled, which will update the server every day at 04:00 AM.

For a better understanding and additional environment variables, check the [mbround18/valheim-docker](https://github.com/mbround18/valheim-docker) repository.

4. **Install the New CasaOS App**  
   Lastly, install the new CasaOS app by pressing the blue install button in the lower right corner:
<div align="left">
<img src="https://raw.githubusercontent.com/Gober-x64/valheim-casaos/main/images/Step_4.png" alt="Step 4">
</div>

Now everything should be set up and functioning. You should be able to join your server.

## Troubleshooting

If, for some reason, you're unable to join your server or you need to troubleshoot, you can open the logs.

- Press the terminal and logs button next to the export button:  
<div align="left">
<img src="https://raw.githubusercontent.com/Gober-x64/valheim-casaos/main/images/Terminal_and_Logs.png" alt="Terminal and Logs Button">
</div>

- Select the Logs tab:  
<div align="left">
<img src="https://raw.githubusercontent.com/Gober-x64/valheim-casaos/main/images/Logs.png" alt="Logs">
</div>
