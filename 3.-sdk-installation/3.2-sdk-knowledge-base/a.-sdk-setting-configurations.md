---
description: >-
  SDK settings are available by modifying the key/value pairs in the
  ModuleConfig.json file.
---

# A. SDK Setting Configurations

Change the value to modify the SDK settings.

{% tabs %}
{% tab title="a. Cutting Range Settings" %}
With the cutting range function, you can specify the minimum and maximum working range by filtering unwanted or out of range images.

1\. In the ModuleConfig.json file, find object A5.

2\. Adjust the distance value. By default, the value for P1 is 10000, P2 is 0.

\- P1 represents the maximum distance.

\- P2 represents the minimum distance.

\- 1000 value represents 1 m of physical distance.

<figure><img src="../../.gitbook/assets/image (6) (1) (1).png" alt=""><figcaption></figcaption></figure>

3. Save the settings and launch your viewer to verify if the change is applied successfully.

<figure><img src="../../.gitbook/assets/image (43).png" alt="" width="298"><figcaption></figcaption></figure>

4\. Here’s a comparison between images with different detection zone.

| Default                                         | Maximum distance < 4 m                                       |
| ----------------------------------------------- | ------------------------------------------------------------ |
| <p>A5->P1: 10000</p><p>A5->P2: 0</p>            | <p>A5->P1: 4000 (4 m)</p><p>A5->P2: 1500 (1.5 m)</p>         |
| ![](<../../.gitbook/assets/image (52).png>)     | ![](../../.gitbook/assets/global\_camera/image%20\(46\).png) |
| ![](<../../.gitbook/assets/image (53) (1).png>) | ![](<../../.gitbook/assets/image (29).png>)                  |
{% endtab %}

{% tab title="b. Flying Pixel Removal" %}
The Flying Pixel Removal function filters noises resulting from the discrepancy between the reflected depth of the object and its background. By default, the Flying Pixel Removal function is enabled.

<figure><img src="../../.gitbook/assets/image (9) (2).png" alt=""><figcaption></figcaption></figure>

1\. In the ModuleConfig.json file, find object A18 > enable\_00000004.

2\. Set the object’s value as true / false to enable / disable the filter.

![](<../../.gitbook/assets/image (61).png>)

3. Save the settings and launch your viewer to verify if the change is applied successfully.

![](<../../.gitbook/assets/image (70).png>)

4. Optionally, change the value of object **P0** for adjusting the filter strength. **0.000000002** represents the strongest filter, while **0.002** represents the weakest.

![](<../../.gitbook/assets/image (47).png>)

5.  Here’s a comparison between images with different levels of filter.

    | P0: 0.000002                                | P0: 0.000004                                | P0: 0.000008                                            |
    | ------------------------------------------- | ------------------------------------------- | ------------------------------------------------------- |
    | ![](<../../.gitbook/assets/image (32).png>) | ![](<../../.gitbook/assets/image (26).png>) | ![](<../../.gitbook/assets/image (41) (1).png>)         |
    | P0: 0.000016                                | P0: 0.000032                                | P0: 0.000064                                            |
    | ![](<../../.gitbook/assets/image (25).png>) | ![](<../../.gitbook/assets/image (38).png>) | ![](<../../.gitbook/assets/image (10) (1) (1) (1).png>) |
{% endtab %}

{% tab title="c. OWCT Setting" %}
Overwrite Confidence Threshold (OWCT) allows users to minimize unfavorable pixels / depth information caused by diffusive refection, resulting in a smoother camera image.

1\. In the ModuleConfig.json file, find object CT.

2\. Under CT, adjust the parameter of ow\_enable. To enable / disable OWCT, type true / false.

![](<../../.gitbook/assets/image (1) (1) (1).png>)

3. Optionally, change the value of object **P0** for adjusting the filter strength. **1** represents the weakest filter, while **10** represents the strongest.\
   By default, the threshold value is 1.

![](<../../.gitbook/assets/image (14) (1).png>)

4. Save the settings and launch your viewer to verify if the change is applied successfully.

![](<../../.gitbook/assets/image (16) (1).png>)

5. Here’s a comparison between images with different confidence threshold level.

| OWCT Level 1                                    | OWCT Level 2                                | OWCT Level 3                                |
| ----------------------------------------------- | ------------------------------------------- | ------------------------------------------- |
| ![](<../../.gitbook/assets/image (15) (1).png>) | ![](<../../.gitbook/assets/image (48).png>) | ![](<../../.gitbook/assets/image (37).png>) |
| OWCT Level 4                                    | OWCT Level 5                                | OWCT Level 6                                |
| ![](<../../.gitbook/assets/image (49).png>)     | ![](<../../.gitbook/assets/image (17).png>) | ![](<../../.gitbook/assets/image (20).png>) |
{% endtab %}

{% tab title="d. Working Range Settings" %}
LIPS Camera supports two working range settings: **Normal Range** (1 \~ 4 m) and **Close Range** (0.2 \~ 1.2 m). You can adjust the working range settings depending on the estimated distance between the camera and the target. By default, the camera works on the Normal Range.

<mark style="color:orange;">Note: Configuration process may vary from model to model.</mark>

1. In the **ModuleConfig.json** file, find object **config**.
2. Under **config**, adjust the parameter of **lens\_mode**. To enable **Normal Range**, type **1**. To enable **Close Range**, type **0**. By default, the value of lens\_mode is 1.

![](<../../.gitbook/assets/image (55).png>)

3. Save the settings and launch your viewer to verify if the change is applied successfully. On the **Calibration column**, parameter beginning with **0203** represents **Normal Range**, and **0211** represents **Close Range** in LIPS SDK.
4. You can also switch between Close and Normal Range instantly by pressing **x**.

![](<../../.gitbook/assets/image (42).png>)
{% endtab %}

{% tab title="e. Output Log Level" %}
LIPS Camera keeps a system log for system activities, warnings, and errors. You can turn the system log ON or OFF by typing Log Level Codes.

1. In ModuleConfig.json, find object debug.
2. Under debug, adjust the value of logLevel. 3 turns the system log ON, and 7 turns the system log OFF.

![](<../../.gitbook/assets/image (68) (1).png>)

3\. Save the settings and launch your viewer to verify if the change is applied successfully.

![](<../../.gitbook/assets/image (11) (1) (1).png>)
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="f. Camera Temperature Display Settings" %}
This feature works for LIPSedge DL only. You can monitor the camera’s temperature on live upon the activation of NiViewer through the Status Window. The recorded temperature will be updated every 10 seconds in Celsius scale (∘C).

1. In ModueConfig.json, find object debug..
2. Under debug, adjust the value of tsensor. To enable / disable temperature display, type true / false.

![](<../../.gitbook/assets/image (57).png>)

3. Save the settings and launch your viewer.
4. On the Status Window, verify if the change is applied successfully.

![](<../../.gitbook/assets/image (12) (1).png>)
{% endtab %}

{% tab title="g. Exposure Frequency Settings" %}
This feature works for LIPSedge DL only. This feature works for LIPSedge DL only. You can match the camera imager’s exposure frequency with the frequency of indoor light source to reduce image flickering. The camera supports 2 frequencies: 50 Hz or 60 Hz.

1\. In ModuleConfig.json, find object camera.

Under camera, adjust the value of anti\_flicker. Type 50 for 50 Hz, 60 for 60 Hz.

![](<../../.gitbook/assets/image (60).png>)

2. Save the settings and launch your viewer to verify if the change is applied successfully.

![](<../../.gitbook/assets/image (62).png>)

3. Here’s a comparison between normal and flickering images.

| Normal Image                                | Flickering Image                            |
| ------------------------------------------- | ------------------------------------------- |
| ![](<../../.gitbook/assets/image (66).png>) | ![](<../../.gitbook/assets/image (67).png>) |
{% endtab %}

{% tab title="h. Orientation Settings" %}
This feature works for LIPSedge DL only. You can rotate the camera’s color or depth image by 90∘.

1. In ModuleConfig.json, find object config.
2. Under config, adjust the value of portrait\_mode\_en. To enable / disable image rotation, type true / false.

![](<../../.gitbook/assets/image (19).png>)

3. Save the settings and launch your viewer to verify if the change is applied successfully.
4. Here’s a comparison between color / depth images with different image orientation settings.

| Horizontal Image                            | Flipped Image                               |
| ------------------------------------------- | ------------------------------------------- |
| ![](<../../.gitbook/assets/image (24).png>) | ![](<../../.gitbook/assets/image (50).png>) |
{% endtab %}

{% tab title="i. Streaming Format Settings" %}
This feature works for LIPSedge DL only. NiViewer supports YUY2 or MJPEG format for color image streaming. You can manage image quality and bandwidth by adjusting the encryption format for color image streaming. YUY2 provides better image quality while costing more bandwidth. On the contrary, MJPEG requires less bandwidth for smoother transmission, but the image quality is less optimal.

1. In ModuleConfig.json, find object config.
2. Under config, adjust the value of ifmt. To enable YUY2 format, type 1. To enable MJPEG format, type 3.

![](<../../.gitbook/assets/image (54).png>)

3. Save the settings and launch your viewer to verify if the change is applied successfully. With YUY2 encryption, the livestream will have slight delay. With MJPEG, the livestream will be smoother.

![](<../../.gitbook/assets/image (7) (1) (1).png>)
{% endtab %}
{% endtabs %}
