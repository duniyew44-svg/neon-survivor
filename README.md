# Neon Survivor - APK

## Yol A: Bilgisayara kurulum gerekmez (GitHub Actions)
1. github.com'da yeni bir depo olustur, bu klasorun icindekileri (.github dahil) yukle.
2. Depoda Actions sekmesi > "Build APK" > bitince "neon-survivor-apk" artifact'ini indir.
3. Zip icindeki app-debug.apk dosyasini telefona at ve kur (Bilinmeyen kaynaklara izin ver).

## Yol B: Kendi bilgisayarinda (Node 20 + JDK 17 + Android Studio)
    npm install
    npx cap add android
    npx cap sync android
    npx cap open android    # Android Studio: Build > Build APK(s)
Dikey kilit icin AndroidManifest.xml'de <activity ...> etiketine android:screenOrientation="portrait" ekle.
