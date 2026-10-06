# Işgärleriň hasaby: Android APK

Bu klasor, `www/index.html` programmasyny GitHub Actions ile Android APK'ya cevirir.
Bilgisayarda Android Studio kurmaniza gerek yok.

## Adimlar
1. https://github.com adresinde yeni bir depo (repository) olusturun (ornegin `isgar-hasaby`). Public veya Private olabilir.
2. Bu klasorun **icindeki her seyi** (`www`, `.github`, `package.json`, `capacitor.config.json`, `.gitignore`) depoya yukleyin.
   - Web arayuzunde: "Add file > Upload files" ile klasorleri surukleyip birakin. `.github` klasorunun yuklendiginden emin olun.
3. Depoda **Actions** sekmesine gidin. Ilk seferde "I understand my workflows, go ahead and enable them" diye sorarsa onaylayin.
4. Soldan **Build Android APK** akisini secin, **Run workflow** dugmesine basin (dosyalari yukledikten sonra kendiliginden de baslar).
5. 4-8 dakika sonra calisma yesil olunca, calismanin sayfasinin altindaki **Artifacts** bolumunden
   `isgarlerin-hasaby-apk` dosyasini indirin. ZIP icinden `app-debug.apk` cikar.
6. APK'yi telefona aktarin ve acin. Android "bilinmeyen kaynaklardan kurulum" izni isteyebilir; izin verin.

## Notlar
- Bu **debug** APK'dir: telefona kurulur, ama Google Play'e yuklenemez. Play Store icin imzali (release) APK/AAB gerekir.
- Excel ve yedek dosyalari telefonda "Paylas" penceresi ile kaydedilir (Dosyalar, Drive, WhatsApp vb. secilir).
- Veriler uygulamanin icinde saklanir. Uygulamayi silerseniz veya verilerini temizlerseniz kaybolur. Duzenli olarak "Ätiýaçlyk nusgasyny al" ile yedek alin.
- Program guncellenirse `www/index.html` dosyasini degistirip depoya yukleyin; APK yeniden olusur.
- Yazdirma (Cap et) telefonda desteklenmez; netijani Excel'e yukleyip oradan yazdirin.
