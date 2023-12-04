# A. Windows Installation(x64)



{% embed url="https://lips-hci.gitbook.io/lips-developer-documentation/installation-and-setup/lipsedge-dl-and-m3-series/installation/windows" fullWidth="false" %}
[https://lips-hci.gitbook.io/lips-developer-documentation/installation-and-setup/lipsedge-dl-and-m3-series/installation/windows](https://lips-hci.gitbook.io/lips-developer-documentation/installation-and-setup/lipsedge-dl-and-m3-series/installation/windows)
{% endembed %}

{% tabs %}
{% tab title="a.	SDK Installation" %}

{% endtab %}

{% tab title="b.	Camera Access by NIViewer" %}
LIPSedge™ DL / M3 utilizes NIViewer, OpenNI’s signature tool, for examining and assessing the quality of depth, RGB, and point cloud image.

&#x20;

1\.        From the Start menu, start NIViewer.

![A screenshot of a computer

Description automatically generated](file:///C:/Users/000311/AppData/Local/Temp/msohtmlclip1/01/clip\_image002.jpg)

&#x20;

2\.        Upon activation, a Status Window, and a Viewer Window both pop

![A screenshot of a computer

Description automatically generated](file:///C:/Users/000311/AppData/Local/Temp/msohtmlclip1/01/clip\_image004.jpg)

\


&#x20;

3\.        The Status Window displays the camera information, such as SDK build version, SDK time stamp, camera ID, status. This example utilizes LIPSedge™ DL.

![Text

Description automatically generated](file:///C:/Users/000311/AppData/Local/Temp/msohtmlclip1/01/clip\_image006.jpg)
{% endtab %}

{% tab title="c. NIViewer Settings" %}
NIViewer relies on hotkeys, which are listed in the help menu, for controlling its functionality and adjustments. By default, the menu in NIViewer is hidden to provide an unobstructed viewing experience. To access this menu, press Shift + ?.

&#x20;

| Note: LIPSedgeTM M3 only supports depth / IR images and functions. IR images will be displayed when functions involving color streaming is selected. |
| ---------------------------------------------------------------------------------------------------------------------------------------------------- |

&#x20;

| Default – The help menu hidden                                                                                                   |
| -------------------------------------------------------------------------------------------------------------------------------- |
| ![一張含有 螢幕擷取畫面, 室內, 瓶子, 藝術 的圖片&#xA;&#xA;自動產生的描述](file:///C:/Users/000311/AppData/Local/Temp/msohtmlclip1/01/clip\_image002.jpg)   |
| The help menu displayed                                                                                                          |
| ![一張含有 螢幕擷取畫面, 文字, 平面設計, 電腦 的圖片&#xA;&#xA;自動產生的描述](file:///C:/Users/000311/AppData/Local/Temp/msohtmlclip1/01/clip\_image004.jpg) |

&#x20;

\


&#x20;

The help menu provides the following functionalities:

&#x20;

u  Depth viewer: Allows the user to observe depth / color images and their image qualities.

u  Point-cloud viewer: Allows the user to observe point-cloud images and their image qualities.

u Screen Layout: Selects the arrangement for multiple camera images between Side by Side or Overlay. With Side by Side layout, depth / color images are displayed side by side. With Overlay, depth / color images are merged and displayed simultaneously.

u Depth: Displays the depth images in various styles or turns the depth image off.

u Color: Select Depth Masked Color to display color images masked with depth grains or select Normal to display regular color images. Select Off to turn the depth image off.

&#x20;

General

u  Show / Hide Help Screen \[Shift + ?]: Shows the Help Screen which contains the description of keyboard shortcuts with their functions.

u  Esc: Exits NIViewer.+
{% endtab %}
{% endtabs %}
