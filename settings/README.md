#Settings

INI files are not a great solution for Android and iOS devices.


But you can use the camera to read a QR code and setup your app.
In this example you can generate a QR code to setup MIS settings.

The logic is:

Generate
Setup MIS->Save to DB->Export JSON->Encrypt->Generate QR

Read:
Read QR->Decrypt QR->JSON Inport to table->Update MIS setting

The DB is generic has possible:
id = 1
s1 -  Mis Server
s2 -  Mis Pass
n1 -  Mis Port
n2 -  Mis Encryption