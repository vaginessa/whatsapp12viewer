# WhatsApp Viewer

Small tool to display chats from the Android WhatsApp database.

## How to use

1. **You need root access to your phone, at least for get the key.** If you don't know what it is: [Wikipedia](https://en.wikipedia.org/wiki/Rooting_%28Android%29)
2. Download your WhatsApp database and key files:
  - /data/data/com.whatsapp/files/key
  - /data/data/com.whatsapp/databases/msgstore.db
  - /data/data/com.whatsapp/databases/wa.db
3. Open WhatsApp Viewer
4. If you aren't root but you have your key file, you can try to use your encrypted database from /sdcard/WhatsApp/Databases/mgstore.db.crypt*, and in Whatsapp Viewer, go to File -> Decrypt (your database extension) and follow the steps
5. File -> Open -> Select file
6. Select msgstore.db in the folder "extracted"
7. Leave account name empty, is was used for older versions of WhatsApp (crypt5)
8. Optional: If you want, you can import contact names from the wa.db file

## Command line support

```
"WhatsApp Viewer.exe" -decrypt12 msgstore-2016-10-22.1.db.crypt12 whatsapp.cryptkey12 decrypted.db
```

You cannot see bigger images because only thumbnails are stored in the database.

## Credits:

* TripCode for crypt12 support https://github.com/EliteAndroidApps/WhatsApp-Crypt12-Decrypter
* Whatsapp Xtract
* pwncrypt5.py https://github.com/aramosf/pwncrypt5/blob/master/pwncrypt5.py
* SQLite
* MD5 http://bobobobo.wordpress.com/2010/10/17/md5-c-implementation/
* UTF8 http://utfcpp.sourceforge.net/
* AES https://polarssl.org/aes-source-code
* Base64 http://www.adp-gmbh.ch/cpp/common/base64.html
* Zlib http://www.zlib.net/
* RapidJSON http://rapidjson.org/
* mbedtls https://github.com/ARMmbed/mbedtls
* Visual Leak Detector https://kinddragon.github.io/vld/

## Special thanks to:

  * [**Andreas-mausch**](https://github.com/andreas-mausch/whatsapp-viewer)
  * [zmeyc](https://github.com/zmeyc/whatsapp-viewer)
