# ZenPhoto CMSv 1.5.7- Authenticated arbitrary file upload to RCE -PoC

##### Dated: 14 Jun 2021 - Author: F-Masood
##### Description: This is a manual way of exploiting the **CVE-2020-36079** vulnerablity which was reported by **Abdulaziz Almisfer**.
##### Need: There was no PoC out, so I made one. 
**̿̿ ̿̿ ̿̿ ̿'̿'\̵͇̿̿\з= ( ▀ ͜͞ʖ▀) =ε/̵͇̿̿/’̿’̿ ̿ ̿̿ ̿̿ ̿̿** 

#### Details
**ZenPhoto CMS version through 1.5.7** is affected by authenticated arbitrary file upload, leading to remote code execution. The attacker must navigate to the uploader plugin, check the elFinder box, and then drag and drop files into the Files(elFinder) portion of the UI. This can, for example, place a .php file in the server's uploaded/ directory.

#### Steps

1. Login to the web portal of ZenCMS.
![alt text](https://github.com/F-Masood/ZenPhotoCMSv1.5.7-RCE/blob/main/001_Login.png)

2. Verify the exact version of ZenCMS.
![alt text](https://github.com/F-Masood/ZenPhotoCMSv1.5.7-RCE/blob/main/002_VersionVerify.png)

3. Navigate to plugins.
![alt text](https://github.com/F-Masood/ZenPhotoCMSv1.5.7-RCE/blob/main/003_Plugins.png)

4. Enable elFinder.
![alt text](https://github.com/F-Masood/ZenPhotoCMSv1.5.7-RCE/blob/main/004_PluginselFinder.png)

5. Now upload a malicious PHP file. 
![alt text](https://github.com/F-Masood/ZenPhotoCMSv1.5.7-RCE/blob/main/006_uploadFile.png)

6. You should have RCE now. 
![alt text](https://github.com/F-Masood/ZenPhotoCMSv1.5.7-RCE/blob/main/007_RCE.png)

#### Video PoC

![](01_zenphoto1.5.7_RCE_POC.gif)
