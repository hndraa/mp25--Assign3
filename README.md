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
   
   `<activity
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
        </activity>`

   ![image](https://github.com/user-attachments/assets/9f4b4947-31b1-4389-a37a-dd16d5cae82a)

10. selanjutnya di Gradle Script > pilih dan buka build.gradle.kts (Modul : app) dan tambahkan kodingan [ `id("kotlin-parcelize")` ]
   ![image](https://github.com/user-attachments/assets/854a8a47-6875-471d-879a-1bdf5b4bf1e1)
![image](https://github.com/user-attachments/assets/4ba0f4e4-e8d0-44d3-883c-fc5f09d37f0a)

12. Selanjutnya jalankan Aplikasi di android studio dengan memilih  Device Manager > pilih perangkat > Run
13. Selamat mencoba!

# Tampilan APP3

## Tampilan Awal
![Screenshot_20250405_133701_Hendra Ahmad Yani - F1D022122 App](https://github.com/user-attachments/assets/8463d6fd-e59a-4a8b-9675-5b720cd91e69)

## Tampilan halaman login jik pw dan email kosong
![Screenshot_20250405_133714_Hendra Ahmad Yani - F1D022122 App](https://github.com/user-attachments/assets/2388e02f-cd78-4698-8eb2-490983e2b04c)

## Tampilan halaman login jika email tidak valid
![Screenshot_20250405_133725_Hendra Ahmad Yani - F1D022122 App](https://github.com/user-attachments/assets/92dbcda2-6c34-4010-ad64-40f98a783b35)

## Tampilan halaman login jika belum registrasi
![Screenshot_20250405_133734_Hendra Ahmad Yani - F1D022122 App](https://github.com/user-attachments/assets/0b852223-01a4-46b5-a28c-74957f387298)

## Tampilan halaman Registrasi dan jika kosong
![Screenshot_20250405_133741_Hendra Ahmad Yani - F1D022122 App](https://github.com/user-attachments/assets/b2b7cb3f-f3e2-4e32-b614-cf9f2a70b786)

## Tampilan halaman registrasi jika format email salah
![Screenshot_20250405_133755_Hendra Ahmad Yani - F1D022122 App](https://github.com/user-attachments/assets/7e2b68fa-ebf5-4e77-aab8-64537413ef73)

## Tampilan halaman registrasi jika panjang password < 8 karakter
![Screenshot_20250405_133804_Hendra Ahmad Yani - F1D022122 App](https://github.com/user-attachments/assets/2075859d-e493-429f-8ff5-2bbcfa2f992e)

## Tampilan Halaman Login setelah register, Jika panjang password < 8 Karakter
![Screenshot_20250405_133819_Hendra Ahmad Yani - F1D022122 App](https://github.com/user-attachments/assets/05ce385f-6357-475c-b241-4aaad2083af3)

## Tampilan Halamann Landingjika berhasil Login
![Screenshot_20250405_133829_Hendra Ahmad Yani - F1D022122 App](https://github.com/user-attachments/assets/c0f49d09-a1f6-4943-a917-c42cc97b9387)
