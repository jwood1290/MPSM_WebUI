# MPSM_WebUI
Updated wifi user interface for MP Select Mini 3D printers

## Description
Slightly revised wifi/web UI from the default MP Slect Mini UI (**screenshots below**). The original UI can be found at: https://www.mpselectmini.com/sample_webui 

## Additions
This UI adds several useful features, including:
  - Total time elapsed during current print
    - If you are were accessing the web UI at the beginning of the print (or send the print command from the UI) the time elapsed will be 
      exact.
    - If you access the UI in the middle of a print, the elapsed print time will be calculated.
  - Estimated time remaining for current print
    - This countdown timer is an estimate of the total time remaining on the print, which is calculated by a running average.
  - Ability to print the "cache.gc" file already on your SD card
    - Useful if you want to reprint something, but do not want to upload the file again.
  - Automatically enables faster wifi uploads (using M563 S5, because S6 is still bugged in the MPSMV2)
  - Added button to allow for a "dry run" (using M111 S14)
    - Allows for testing print travels without extruding filament or heating the hotend/bed.
  - Added button to turn off "dry run" option (using M111 S0)
  - Edited colors of the extruder movement icons for better consistency (separated directions with individual colors)
  - Added icons of movement directions (e.g. forward, backward, left, right, etc.) for clarity
  - Added target temperature range markers to temperature graphs (extruder and bed)
  
Most of the revisions are cosmetic and do not alter any settings on your printer (other than file upload speed). This has been tested on a MP Select Mini V2. 

**Note: Requires UI Controller firmware version 42 or greater to enable a custom Web UI.**

## Preview
![webui_top](https://user-images.githubusercontent.com/38746964/39291075-657c5850-48f7-11e8-9b73-845e2bd68429.jpg) 
![webui_bottom](https://user-images.githubusercontent.com/38746964/39291441-9cfc3b8c-48f8-11e8-8168-15e690784c4f.jpg)
