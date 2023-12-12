# A.  OpenNI2 and Dependent Files

The LIPSedge ™ SDK (OpenNI based) consists of two main components: OpenNI2 folder and other dependent folder/files .&#x20;

Except for the OpenNI2 folder, all the rest of the files are dependent folder/files.

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

{% tabs %}
{% tab title="OpenNI2 and Dependent folders/Files" %}
* NOTICE : Dependent libraries necessary for LIPSedge ™ SDK functionality. Do NOT modify or delete the folder content.&#x20;
* OpenNI2 : OpenNI related files that are essential for camera integration and function control, including system configuration files and example applications.&#x20;
* Auxiliary files : Supplementary information for the LIPSedge ™ SDK. \
  − EULA\_LIPS\_SDK.txt : The end user agreement.\
  − LIPS.ico : LIPS Corp.’s icon which appears during application operation. \
  − ReleaseNotes : Announcement of the latest feature.
* Uninstallation components : Run unins000.exe for uninstallation. Note that unins000.dat must be present.
{% endtab %}

{% tab title="OpenNI2 Folder" %}
The SDK package for LIPSedge ™ provides a comprehensive set of files and folders to support camera integration and development.&#x20;

These resources include OpenNI C++ API documentation, header files, libraries for compilation, sample applications, system files, and important information such as licenses and release notes.&#x20;

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

* Documentation : Contains essential OpenNI C++ API documentation.
* Include : Contains essential OpenNI C++ headers. These headers can be checked along with the associated library files to facilitate development.&#x20;
* Lib : Contains library files, specifically OpenNI2.lib and realsenses2.lib. These libraries are used in conjunction with MS Visual Studio C++ for compilation.&#x20;
* LIPSedgeSamples : Contains a series of executable tools and the source code of these tools.&#x20;
* Redist : Contains network configuration files, camera drivers and system files necessary for image streaming.&#x20;
* Tools : Holds captured frames from example programs and other camera configuration files.&#x20;
* CHANGES : The change log for OpenNI.
* LICENSE : Contains information about the licensing terms for the SDK.
* NOTICE : Contains copyright and attribution notices relevant to the OpenNI components.&#x20;
* ReleaseNotes : The latest system requirements for OpenNI.
{% endtab %}
{% endtabs %}
