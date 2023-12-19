# B. Linux/Ubuntu Installation(x64)

{% tabs %}
{% tab title="a. SDK Installation" %}
To access the SDK, visit [https://www.lips-hci.com/3d-camera](https://www.lips-hci.com/3d-camera) and procure the package for the preferred version, framework, and compatible operating system.

1. Visit [LIPSedge™ SDK](https://www.lips-hci.com/developer-documentation) website.
2. Select the installation file based on the compatible operating system and download the installation file.

![](<../../.gitbook/assets/global_camera/LinuxUbuntu Installation/0 (3).png>)

3. Start **terminal** and go to **the installation file’s location**. In this example, /home is used.
4. Change the **access permission** of the installation file.

<mark style="background-color:green;">**chmod +x LIPSedge-Camera-SDK-Linux-1.01.run**</mark>

![](<../../.gitbook/assets/global_camera/LinuxUbuntu Installation/1 (1).png>)

5. Execute the installation file.

<mark style="background-color:green;">**./LIPSedge-Camera-SDK-Linux-1.01.run**</mark>

![](<../../.gitbook/assets/global_camera/LinuxUbuntu Installation/2 (1).png>)

6. The file will be decompressed into model-specific installation files.

<figure><img src="../../.gitbook/assets/global_camera/LinuxUbuntu Installation/image.png" alt=""><figcaption></figcaption></figure>

7. Go to **the folder with the installation file for the intended model** and execute the installation file. In this example, LIPSedge-DL-SDK-Linux-amd64-2.4.4.2\_v1.8.2.xz.run is used.

<mark style="background-color:green;">**./LIPSedge-DL-SDK-Linux-amd64-2.4.4.2\_v1.8.2.xz.run**</mark>

![](<../../.gitbook/assets/global_camera/LinuxUbuntu Installation/4 (1).png>)

8. Press **Y**.

![](<../../.gitbook/assets/global_camera/LinuxUbuntu Installation/5 (1).png>)

9. Select **Install**.

![](<../../.gitbook/assets/global_camera/LinuxUbuntu Installation/6 (1).png>)

10. Once the installation is successful, the LIPSedge™ SDK and its relevant components is accessible at the **installation location**. In this example, the installation location is ./home. For the folder content, refer to similar content in _3.2-A-a. OpenNI2 and Dependent Files._

![](<../../.gitbook/assets/global_camera/LinuxUbuntu Installation/7 (1).png>)
{% endtab %}

{% tab title="b. Camera Access by NIViewer" %}
LIPSedge™ DL / M3 utilizes NIViewer, OpenNI’s signature tool, for examining and assessing the quality of depth, RGB, and point cloud image.

1. Go to **LIPSedge-Camera-SDK-Linux > LIPSedge-\[Model]-SDK** and start NIViewer.

![](<../../.gitbook/assets/global_camera/LinuxUbuntu Installation/8 (1).png>)

2. Upon activation, a **Status Window**, and a **Viewer Window** both pop

![](<../../.gitbook/assets/global_camera/LinuxUbuntu Installation/9 (1).png>)

3. The **Status Window** displays the camera information, such as SDK build version, SDK time stamp, camera ID, status.

![](<../../.gitbook/assets/global_camera/LinuxUbuntu Installation/10 (1).png>)

4. The **Viewer Window** displays the Depth image on screen.

<figure><img src="../../.gitbook/assets/global_camera/LinuxUbuntu Installation/image (22).png" alt=""><figcaption></figcaption></figure>

5. Press **\[p]** to activate **the pointer mode**. The meter below shows the depth data of the given point marked by the indicator.

![](<../../.gitbook/assets/global_camera/LinuxUbuntu Installation/12 (1).png>)

6. Optionally choose an area to display by dragging a cropping area with the cursor. The rest of the areas will be masked from displaying.

![](<../../.gitbook/assets/global_camera/LinuxUbuntu Installation/13 (1).png>)

7. Optionally press F to maximize / minimize the viewer’s window.

**Note**: If for any reason the USB cable is forcibly removed while NiViewer is functioning, an **ERROR! Device disconnected** message appears on the screen. To resume livestreaming, re-plug the USB cable.

![](<../../.gitbook/assets/global_camera/LinuxUbuntu Installation/14 (1) (1).png>)

8. Optionally press C to capture the current screen as a raw format file. To access the raw format file, go to **LIPSedge™ DL\_M3 SDK > OpenNI2 > Tools > CaptureFrames** and drag the captured image file to the **Ni2RawViewer.exe**. For details, refer to _5.1 LIPSedgeSamples_.

![](<../../.gitbook/assets/global_camera/LinuxUbuntu Installation/15 (1).png>)

9. If by accident the camera is abruptly connected, the camera will automatically restore the camera connection.

![](<../../.gitbook/assets/global_camera/LinuxUbuntu Installation/16 (1).png>)
{% endtab %}

{% tab title="c. NIViewer Settings" %}
NIViewer relies on hotkeys, which are listed in the help menu, to control its functionality and adjustments.&#x20;

The hotkey functions for the NIViewer of Linux version are identical to its Windows counterpart. Refer to _3.1-A-c. NIViewer Settings_ for details.
{% endtab %}

{% tab title="d. IP Address Configuration" %}
This section is NOT applicable to this model.
{% endtab %}
{% endtabs %}

