
# GPU Issue Description

I'm having an issue with my gpu not showing up in Settings > Display > Graphics settings > ANY_DEVICE_HERE > Options

In that my dedicated GPU (NVIDIA GeForce GTX 660 Ti) is not showing up in Options


# What I've tried:

1) Verified that my GPU is available in Device manager
2) Verified that its drivers are up to date in Device manager > Display Adapters
3) Verified that the GPU is operating correctly via Device manager
4) Installed any driver updates available for my GPU from NVIDIA's website:
   1) Installed Game Ready Driver (GRD): 474.14-desktop-win10-win11-64bit-international-dch-whql.exe
   2) Studio Driver: None available
5) Verified the GPU is not being disabled by the Windows system power settings
6) Verified in BIOS that the GPU is selected as the primary graphics processor and that the correct slot was selected
7) Verified that the issue persists in safe mode
8) Verified motherboard using the latest version of BIOS

# My Environment Specifications

## Windows Device Specifications:

- Device name	Damien3
- Processor	Intel(R) Core(TM) i5-3570K CPU @ 3.40GHz   3.40 GHz
- Installed RAM	16.0 GB (15.9 GB usable)
- System type	64-bit operating system, x64-based processor
- Pen and touch	No pen or touch input is available for this display

## Windows Specifications:

- Edition	Windows 10 Pro
- Version	21H2
- Installed on 11/22/2020
- OS build	19044.2364
- Experience	Windows Feature Experience Pack 120.2212.4190.0

## Motherboard
- ASRock Z77 Extreme4

# TOP PART OF DxDiag REPORT (the full report is over 2000 lines):

------------------
System Information
------------------

```
      Time of this report: 12/26/2022, 15:26:28
             Machine name: DAMIEN3
               Machine Id: {919C71A6-CE3D-48F8-88C3-540B1B0C4172}
         Operating System: Windows 10 Pro 64-bit (10.0, Build 19044) (19041.vb_release.191206-1406)
                 Language: English (Regional Setting: English)
      System Manufacturer: To Be Filled By O.E.M.
             System Model: To Be Filled By O.E.M.
                     BIOS: BIOS Date: 03/12/18 12:20:40 Ver: 04.06.05 (type: BIOS)
                Processor: Intel(R) Core(TM) i5-3570K CPU @ 3.40GHz (4 CPUs), ~3.4GHz
                   Memory: 16384MB RAM
      Available OS Memory: 16266MB RAM
                Page File: 9935MB used, 11451MB available
              Windows Dir: C:\Windows
          DirectX Version: DirectX 12
      DX Setup Parameters: Not found
         User DPI Setting: 120 DPI (125 percent)
       System DPI Setting: 144 DPI (150 percent)
          DWM DPI Scaling: UnKnown
                 Miracast: Available, no HDCP
Microsoft Graphics Hybrid: Not Supported
 DirectX Database Version: 1.0.8
           DxDiag Version: 10.00.19041.2075 64bit Unicode
```

------------
DxDiag Notes
------------
      Display Tab 1: No problems found.
      Display Tab 2: No problems found.
      Display Tab 3: No problems found.
        Sound Tab 1: No problems found.
        Sound Tab 2: No problems found.
        Sound Tab 3: No problems found.
        Sound Tab 4: No problems found.
          Input Tab: No problems found.

--------------------
DirectX Debug Levels
--------------------
```
Direct3D:    0/4 (retail)
DirectDraw:  0/4 (retail)
DirectInput: 0/5 (retail)
DirectMusic: 0/5 (retail)
DirectPlay:  0/9 (retail)
DirectSound: 0/5 (retail)
DirectShow:  0/6 (retail)
```
---------------
Display Devices
---------------
```
           Card name: NVIDIA GeForce GTX 660 Ti
        Manufacturer: NVIDIA
           Chip type: NVIDIA GeForce GTX 660 Ti
            DAC type: Integrated RAMDAC
         Device Type: Full Device (POST)
          Device Key: Enum\PCI\VEN_10DE&DEV_1183&SUBSYS_841F1043&REV_A1
       Device Status: 0180200A [DN_DRIVER_LOADED|DN_STARTED|DN_DISABLEABLE|DN_NT_ENUMERATOR|DN_NT_DRIVER]
 Device Problem Code: No Problem
 Driver Problem Code: Unknown
      Display Memory: 10131 MB
    Dedicated Memory: 1998 MB
       Shared Memory: 8133 MB
        Current Mode: 1920 x 1080 (32 bit) (60Hz)
```

# HWINFO GPU REPORT

Video Chipset
Video Chipset:                                                                  NVIDIA GeForce GTX 660 Ti
Video Chipset Codename:                                                         GK104-300
Video Memory:                                                                   2048 MBytes of GDDR5 SDRAM [Hynix]

Video Card
Video Card:                                                                     ASUS GTX660 TI DirectCU II OC
Video Bus:                                                                      PCIe v3.0 x16 (8.0 GT/s) @ x16 (2.5 GT/s)
Video RAMDAC:                                                                   Integrated RAMDAC
Video BIOS Version:                                                             80.04.4b.00.5b
Video Chipset Revision:                                                         A1

Performance
Graphics Processor Clock:                                                       324.0 MHz
Video Unit Clock:                                                               405.0 MHz
Graphics Memory Clock:                                                          162.0 MHz (Effective 648.0 MHz)
Graphics Memory Bus Width:                                                      192-bit
Number Of ROPs:                                                                 24
Number Of Unified Shaders:                                                      1344
Number Of TMUs (Texture Mapping Units):                                         112

ASIC Manufacturer:                                                              TSMC
ASIC Type:                                                                      Qualification/Production Part
ASIC Quality:                                                                   77.2 %
ASIC Serial Number:                                                             3242337745
NVIDIA SLI Status:                                                              Not Present

Resizable BAR (ReBAR) Support:                                                  Not Supported

Hardware ID:                                                                    PCI\VEN_10DE&DEV_1183&SUBSYS_841F1043&REV_A1
PCI Location (Bus:Dev:Fnc):                                                     1:00:0

Driver Information
Driver Manufacturer:                                                            NVIDIA
Driver Description:                                                             NVIDIA GeForce GTX 660 Ti
Driver Provider:                                                                NVIDIA
Driver Version:                                                                 27.21.14.5671 (GeForce 456.71)
Driver Date:                                                                    29-Sep-2020
DCH/UWD Driver:                                                                 Capable
DeviceInstanceId                                                                PCI\VEN_10DE&DEV_1183&SUBSYS_841F1043&REV_A1\4&15001D53&0&0008
Location Paths                                                                  PCIROOT(0)#PCI(0100)#PCI(0000)




# Instructions & Steps

## Starting your computer in Safe Mode

1. Close any open programs and save your work.
2. Press the Windows key + R on your keyboard to open the Run dialog box.
3. Type "msconfig" into the Run dialog box and hit Enter. This will open the System Configuration utility.
4. In the System Configuration utility, go to the "Boot" tab.
5. Under "Boot options", check the box next to "Safe boot" and select "Minimal" from the drop-down menu.
6. Click on the "Apply" button, and then click on the "OK" button.
7. The system will prompt you to restart your computer. Click on the "Restart" button to restart your computer in Safe Mode.

- When your computer starts up in Safe Mode, you will see the words "Safe Mode" in all four corners of the screen. This indicates that you are running in Safe Mode. You can use Safe Mode to troubleshoot issues with your system or to install or uninstall software. When you are finished, you can restart your computer and boot into normal mode by repeating the steps above and unchecking the "Safe boot" option.


## Links open just before giving up
- [answers.microsoft](https://answers.microsoft.com/en-us/windows/forum/all/unable-to-select-gpu-in-windows-graphics-settings/7c879d69-d482-4734-8709-33a54f4a5c78)
- [obsproject.com](https://obsproject.com/wiki/Laptop-Troubleshooting)
- [chat.openai](https://chat.openai.com/chat/310c0027-ea8e-42b5-8940-74225d7b9d45)
- [obsproject.com](https://obsproject.com/forum/threads/unable-to-do-recording.125350/)
- [github.com](https://github.com/GigglePocket/OBS_Error#system-information)
- [obsproject.com](https://obsproject.com/wiki/General-Performance-and-Encoding-Issues)
- [gist.github](https://gist.github.com/4144/143998ee073c009d31bc0de86f53b286)
- [www.google](https://www.google.com/search?q=does+discord+markdown+support+hyperlinks%3F&rlz=1C1RXQR_enUS928US928&sxsrf=ALiCzsYeKhT7bnXNP0vHuqakcKui1x7n_Q%3A1672108740176&ei=xFqqY6uxCs_k0PEP4aOSQA&ved=0ahUKEwiro--74pj8AhVPMjQIHeGRBAgQ4dUDCBA&uact=5&oq=does+discord+markdown+support+hyperlinks%3F&gs_lcp=Cgxnd3Mtd2l6LXNlcnAQAzIFCCEQoAEyBQghEKABMgUIIRCgATIFCCEQoAEyBQghEKsCMgUIIRCrAjIFCCEQqwI6CggAEEcQ1gQQsAM6BAgAEEM6CggAELEDEIMBEEM6CwguEIAEELEDEIMBOhEILhCABBCxAxCDARDHARDRAzoLCAAQgAQQsQMQgwE6CAgAEIAEELEDOg4ILhCxAxCDARDHARDRAzoFCAAQkQI6DgguEIAEELEDEMcBENEDOgQIIxAnOggIABCxAxCDAToFCAAQgAQ6CwguEIAEEMcBEK8BOgQIABADOgoIABCABBCHAhAUOgYIABAWEB46BQgAEIYDOgcIABCABBANOggIABAIEB4QDToFCAAQogRKBAhBGABKBAhGGABQnBRYs1tgpF5oAXABeACAAYkBiAGxHJIBBDMyLjmYAQCgAQHIAQjAAQE&sclient=gws-wiz-serp)
- [help.elgato](https://help.elgato.com/hc/en-us/articles/360027954992-Which-NVIDIA-graphic-cards-do-support-NVENC-technology-)
- [en.wikipedia](https://en.wikipedia.org/wiki/List_of_Nvidia_graphics_processing_units)
- [github.com](https://github.com/obsproject/obs-studio/releases/tag/29.0.0-beta3)