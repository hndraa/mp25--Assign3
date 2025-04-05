# mp25--Assign3
## Aplikasi Login-Register Sederhana
File ini adalah file kt dan xml untuk project bernama App3 di android studio untuk menjalankan code ini:
1. Buka android studio pilih _new project_ lalu pilih _new activity_ beri nama app3 dan next.
2. Ubah tampilan dari PROJECT ke  ANDROID
   
   ![image](https://github.com/user-attachments/assets/59d65576-2f1a-415c-9032-1f9fd5884e0e)

4. lalu di bagian App > kotlin+java > com.example.app3 , masukan file "User.kt", "login.kt", "register.kt", "landing.kt".
   
   ![image](https://github.com/user-attachments/assets/9eb8c1f8-b54c-4abb-a327-ca6d0aeab0e2)

6. selanjutnya bagian App > res > Layout, masukan file "activity_login.xml", "activity_register.xml", "activity_landing.xml".

   ![image](https://github.com/user-attachments/assets/cebc8db2-a8ce-4254-9b0b-50f489fc0d54)

8. Buka lagi App > manifests > AndroidManifest.xml > tambahkan codingan berikut:
      
    ```  kotlin
   <activity
               android:name=".landing"
               android:exported="false" />
           <activity
               android:name=".register"
               android:exported="false" />
           <activity
               android:name=".login"
               android:exported="true"> <!-- Set TRUE & tambahkan intent-filter -->
               <intent-filter>
                   <action android:name="android.intent.action.MAIN" />
                   <category android:name="android.intent.category.LAUNCHER" />
               </intent-filter>
           </activity>


![image](https://github.com/user-attachments/assets/9f4b4947-31b1-4389-a37a-dd16d5cae82a)

10. selanjutnya di Gradle Script > pilih dan buka build.gradle.kts (Modul : app) dan tambahkan kodingan [ `id("kotlin-parcelize")` ]
    
   ![image](https://github.com/user-attachments/assets/854a8a47-6875-471d-879a-1bdf5b4bf1e1)
   
   ![image](https://github.com/user-attachments/assets/4ba0f4e4-e8d0-44d3-883c-fc5f09d37f0a)

12. Selanjutnya jalankan Aplikasi di android studio dengan memilih  Device Manager > pilih perangkat > Run
13. Selamat mencoba!

# Tampilan APP3

## Tampilan Awal
![image](https://github.com/user-attachments/assets/5cf402f8-643c-4a8b-80ee-3dfe8fa01379)

## Tampilan halaman login jik pw dan email kosong
![image](https://github.com/user-attachments/assets/f6740b58-3009-4a71-be30-178bc6ca4f57)

## Tampilan halaman login jika email tidak valid
![image](https://github.com/user-attachments/assets/d24820d1-a911-4c08-a631-7e950679078a)

## Tampilan halaman login jika belum registrasi
![image](https://github.com/user-attachments/assets/167af7c1-7272-429d-9bb9-f287fc80abb5)

## Tampilan halaman Registrasi dan jika kosong
![image](https://github.com/user-attachments/assets/979cbf71-02fd-46cf-8d7f-583e17cabce1)

## Tampilan halaman registrasi jika format email salah
![image](https://github.com/user-attachments/assets/1bc1f6b2-8c32-416f-acc6-f93c51648ef2)

## Tampilan halaman registrasi jika panjang password < 8 karakter
![image](https://github.com/user-attachments/assets/4381e014-0bd3-429d-9ad3-b1969f440b12)

## Tampilan Halaman Login setelah register, Jika panjang password < 8 Karakter
![image](https://github.com/user-attachments/assets/d9553be7-64c5-4404-9eb9-4538b4d34cf0)

## Tampilan Halamann Landingjika berhasil Login
![image](https://github.com/user-attachments/assets/416671f5-3e95-4add-a022-0c0175ed8a84)
