# Valheim CasaOS

This repository helps you run a Valheim server on CasaOS.

The recommended YAML configuration, `Valheim-server_mbround.yaml`, is based on the repository [mbround18/valheim-docker](https://github.com/mbround18/valheim-docker).  
Inspiration was also taken from this [Reddit post](https://www.reddit.com/r/valheim/comments/1bijg8x/valheim_in_casaos/).

## Installation Guide

1. **Download or Copy the YAML Configuration File**  
   Download or copy the content of this [YAML configuration file](https://github.com/Gober-x64/valheim-casaos/blob/main/Valheim-server_mbround.yaml).

2. **Install on CasaOS**  
   - Press the "+" sign and click on "Install a customized app".  
     ![Step 1](https://raw.githubusercontent.com/Gober-x64/valheim-casaos/main/images/Step_1.png)

   - In the new window, click on the import symbol in the upper right corner, next to the "X" symbol.  
     ![Step 2](https://raw.githubusercontent.com/Gober-x64/valheim-casaos/main/images/Step_2.png)

   - In the import window, drag and drop the downloaded file into the upload section in the lower half of the window, or copy the content of the `.yaml` file into the text box above. Press the submit button.  
     ![Step 3](https://raw.githubusercontent.com/Gober-x64/valheim-casaos/main/images/Step_3.png)

3. **Change the Following Environment Variables**  
   ![Change this](https://raw.githubusercontent.com/Gober-x64/valheim-casaos/main/images/Change_This.png)  

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
   ![Step 4](https://raw.githubusercontent.com/Gober-x64/valheim-casaos/main/images/Step_4.png)

Now everything should be set up and functioning. You should be able to join your server.

## Troubleshooting

If, for some reason, you're unable to join your server or you need to troubleshoot, you can open the logs.

- Press the terminal and logs button next to the export button:  
  ![Terminal and Logs Button](https://raw.githubusercontent.com/Gober-x64/valheim-casaos/main/images/Terminal_and_Logs.png)

- Select the Logs tab:  
  ![Logs](https://raw.githubusercontent.com/Gober-x64/valheim-casaos/main/images/Logs.png)
