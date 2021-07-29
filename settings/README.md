# Settings

INI files are not a great solution for Android and iOS devices.


But you can use the camera to read a QRcode and setup your app.

This way you can even send your QRcode my email/chat!

In this example you can generate a QR code to setup MIS settings.

The logic is:

### 1st Run
Get all MIS Settings and add them to the DB.
If is not the first time will get settings from the DB and load to MIS Settings (Communication Profile)

### Generate:
Export JSON from DB->Encrypt->Generate QR

### Read:
Read QR->Decrypt QR->JSON Inport to table->Update MIS setting


The DB is generic has possible, this way you can also use to set up external DB details

* id = 1
* s1 -  Mis Server
* s2 -  Mis Pass
* n1 -  Mis Port
* n2 -  Mis Encryption
