# Keolapse Module Installation Guide

## Initial Setup

1. SSH into your AllSky system
2. Create the module file by running:
   ```bash
   nano /opt/allsky/modules/allsky_keolapse.py
   ```

## Adding the Module Code

1. Copy the Python code from the Module python code in this repository:
   * Open the Python file in a text editor on your computer
   * Select all text (CTRL+A or CMD+A on Mac)
   * Copy the text (CTRL+C or CMD+C)
2. Paste into the SSH window:
   * Click in the nano editor window
   * Paste the code (CTRL+V or CMD+V)
3. Save and exit:
   * Press CTRL+X
   * Press Y to confirm saving
   * Press Enter to confirm the filename.

## Set Execution Permissions

Make the module executable:
```bash
chmod +x /opt/allsky/modules/allsky_keolapse.py
```

## Configure in AllSky WebUI

1. Open AllSky's web interface in your browser
2. Navigate to the "Modules" tab
3. Select "Periodic" from the dropdown menu
4. Drag the Keolapse module to the right side
5. Click "Settings" to configure the module parameters

## Testing

* Use the "Generate Test Data" option in the testing tab of the module
* This creates sample data and makes it easier to verify the correct output

## Accessing Output Files

To access the Keolapse test images and videos, you have two options:

### Option 1: FTP Transfer
Transfer files from your AllSky to your computer using an FTP client

### Option 2: SAMBA Installation (Highly Recommended)
Setting up SAMBA allows you to access your AllSky files directly through your computer's file explorer:

1. Install SAMBA using the guide at: https://github.com/jcauthen78/Allsky-Samba
2. This setup assumes default installation with "Pi" as the username
3. After installation, you can browse AllSky files directly from your computer

> **Note:** SAMBA is highly recommended for all users as it simplifies file access significantly.

## Troubleshooting

If you encounter any issues during installation or have questions about the instructions, please send me a message.