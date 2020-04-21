

# Sending a Payload

> [!WARNING|label:If you are here to test if your Switch is patched]
> Make sure you have [put your device into RCM](user_guide/emummc/entering_rcm.md) and downloaded Hekate (if necessary, extract its zip file onto the root of your SD card) before continuing. Once finished, if your console is **not** patched, continue with [Partitioning the SD](user_guide/emummc/partitioning_sd.md).

> [!DANGER|label:If nothing happens after you send the payload]
>    If your console's screen remains black after you've sent Hekate, it's possible your payload was corrupted, or that your console is patched. If your payload injector program shows that 0 bytes were sent, then it is definitely patched, so you'll be unable to proceed with the rest of the guide.

Now that the device is in RCM, we will need to send it a payload. The methods are mostly the same, but slightly differ depending on what hardware you have available.

<!-- tabs:start -->

#### **Windows**

> [!TIP|label:What you need]
>    - The latest release of <a href="https://github.com/eliboa/TegraRcmGUI/releases" target="_blank">TegraRcmGUI</a> (either the MSI or zip)
>    - A USB-A to USB-C cable (or a standard USB-C cable if your computer natively supports USB-C)
>
>    Payloads you'll need for this guide:
>
>    - The latest release of <a href="https://github.com/CTCaer/hekate/releases/" target="_blank">Hekate</a> (either the hekate_ctcaer bin or the hekate_ctcaer zip)
>    - The latest release of <a href="https://github.com/suchmememanyskill/TegraExplorer/releases" target="_blank">TegraExplorer</a>

> [!NOTE|label:Instructions]
>    1. Install and run TegraRcmGUI.
>    2. Navigate to the `Settings` tab, then press `Install Driver` and follow the on-screen instructions.
>    3. Connect your Switch in RCM to your PC using the USB cable.
>    4. Navigate to the `Payload` tab of TegraRcmGUI.
>        - Your Switch should be shown as detected in the bottom left corner.
>    5. Press the file button next to `Inject payload`, and navigate to and select your payload `.bin` file.
>        - The first time you read this page you should inject TegraExplorer.bin.
>    6. Click `Inject payload` to launch the payload you selected.

&nbsp;
#### **MacOS**

> [!TIP|label:What you need]
>    - The latest release of <a href="https://github.com/nh-server/fusee-interfacee-tk/releases" target="_blank">fusee-interfacee-tk</a>
>    - A USB-A to USB-C cable (or a standard USB-C cable if your computer natively supports USB-C)
>
>    Payloads you'll need for this guide:
>
>    - The latest release of <a href="https://github.com/CTCaer/hekate/releases/" target="_blank">Hekate</a> (either the hekate_ctcaer bin or the hekate_ctcaer zip)
>    - The latest release of <a href="https://github.com/suchmememanyskill/TegraExplorer/releases" target="_blank">TegraExplorer</a>

> [!NOTE|label:Instructions]
>    1. Download and run the payload injector (if you are on Linux, you will need to run this program as root or use `sudo`).
>    2. Connect your Switch in RCM to your PC using the USB cable.
>    3. Wait for your Switch to be shown as found in the injector.
>    4. Press `Select Payload`, and navigate to and select your payload `.bin` file.
>        - The first time you read this page you should inject TegraExplorer.bin.
>    5. Click `Send Payload!` to launch the payload you selected.

&nbsp;
#### **Android**

> [!TIP|label:What you need]
>    - The latest release of <a href="https://github.com/MenosGrante/Rekado/releases" target="_blank">Rekado</a>
>        - You will need to enable Unknown Sources in your device settings to install this
>    - A USB-C cable
>        - If your device has a USB-C port, you may use a C-C cable
>        - If your device only has a Micro USB port, you will need a USB OTG adapter and a USB A-C cable
>            - This **will not work** on every phone!
>
>    Payloads you'll need for this guide:
>
>    - The latest release of <a href="https://github.com/CTCaer/hekate/releases/" target="_blank">Hekate</a> (either the hekate_ctcaer bin or the hekate_ctcaer zip)
>    - The latest release of <a href="https://github.com/suchmememanyskill/TegraExplorer/releases" target="_blank">TegraExplorer</a>
		
> [!NOTE|label:Instructions]
>    1. Copy the hekate_ctcaer `.bin` file from the Hekate `.zip` file to a location on your phone.
>        - A tool such as Amaze File Manager can do this.
>    2. Launch Rekado on your phone.
>    3. Navigate to `Payloads`, then press the `+` button at the bottom right.
>    4. Navigate to your hekate_ctcaer `.bin` file and tap it to add it to Rekado's menu.
>    5. **Optional, but recommended**: Navigate to Rekado's settings and enable `Hide bundled`.
>    6. Connect your Switch in RCM to your phone using the USB cable.
>    7. If prompted, grant Rekado access to the Switch.
>    8. Select your payload `.bin` file in the dialog that pops up.
>        - The first time you read this page you should inject TegraExplorer.bin.


#### **Chomebook**

> [!TIP|label:What you need]
>    - A USB-C cable
>    - If your chromebook has a USB-C port, do note that this will not work using a C-C cable.
>
>    Payloads you'll need for this guide:
>
>    - The latest release of <a href="https://github.com/CTCaer/hekate/releases/" target="_blank">Hekate</a> (either the hekate_ctcaer bin or the hekate_ctcaer zip)
>    - The latest release of <a href="https://github.com/suchmememanyskill/TegraExplorer/releases" target="_blank">TegraExplorer</a>

> [!NOTE|label:Instructions]
>    1. Go to the injection [website](https://switchgui.de/web-payload/) and scroll all the way down
>    2. Select the "Upload Payload" option and upload the hekate_ctcaer `.bin` file from the Hekate `.zip` file.
>        - The first time you read this page you should inject TegraExplorer.bin.
>    3. Connect your Switch in RCM to your Chromebook using the USB cable.
>    4. Select "Do the thing". A pop up will appear. Click the `APX` option.
>    5. Press the Connect button and the payload will be injected.

<!-- tabs:end -->

-----

### [Continue to Partitioning the SD <i class="fa fa-arrow-circle-right fa-lg"></i>](user_guide/emummc/partitioning_sd.md) {docsify-ignore}
