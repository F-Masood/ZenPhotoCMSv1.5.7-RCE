# ZenPhoto CMSv 1.5.7- Authenticated arbitrary file upload to RCE -PoC

##### Dated: 14 Jun 2021 - Author: F-Masood
##### Description: This is a manual way of exploiting the **CVE-2020-36079** vulnerablity.
##### Need: There was no PoC out, so I made one. **̿̿ ̿̿ ̿̿ ̿'̿'\̵͇̿̿\з= ( ▀ ͜͞ʖ▀) =ε/̵͇̿̿/’̿’̿ ̿ ̿̿ ̿̿ ̿̿** 

#### Details
Zenphoto through 1.5.7 is affected by authenticated arbitrary file upload, leading to remote code execution. The attacker must navigate to the uploader plugin, check the elFinder box, and then drag and drop files into the Files(elFinder) portion of the UI. This can, for example, place a .php file in the server's uploaded/ directory.
