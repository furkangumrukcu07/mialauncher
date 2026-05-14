# Mia Launcher — Play Store gizlilik politikası (GitHub Pages)

Bu klasör, Google Play Console’da **Gizlilik politikası URL’si** olarak kullanmak üzere hazırlanmış statik sayfalardır.

## `https://github.com/furkangumrukcu07/miaplayer` reposuna kopyalama

Bu ortamdan sizin GitHub hesabınıza **doğrudan push yapılamaz**; aşağıdaki adımları kendi makinenizde uygulayın.

1. GitHub’da `furkangumrukcu07/miaplayer` deposunu oluşturun veya mevcut repoyu açın.
2. Bu klasördeki dosyaları repoya kopyalayın. **GitHub Pages** için önerilen yapı:
   - **Seçenek A — yalnızca gizlilik sayfası (en kısa URL):**  
     `index.html` ve `privacy-policy-en.html` dosyalarını repoda **`docs/`** köküne koyun:  
     `miaplayer/docs/index.html`  
     Sonra: **Settings → Pages → Build and deployment → Branch: `main` / Folder: `/docs`**  
     Play Store URL’si: `https://furkangumrukcu07.github.io/miaplayer/`
   - **Seçenek B — alt yol:**  
     `docs/privacy/index.html` olarak koyarsanız URL:  
     `https://furkangumrukcu07.github.io/miaplayer/privacy/`  
     (Bu durumda `index.html` içindeki İngilizce linki `./privacy-policy-en.html` yerine gerçek konuma göre güncelleyin.)

3. Birkaç dakika sonra sayfa yayına alınır; tarayıcıda açıp metni kontrol edin.
4. Play Console’da **Uygulama içeriği → Gizlilik politikası** alanına yukarıdaki `https://furkangumrukcu07.github.io/miaplayer/` (veya seçtiğiniz tam yol) adresini yazın.

## Dosyalar

| Dosya | Açıklama |
|--------|-----------|
| `index.html` | Türkçe gizlilik politikası + Lawnchair / AOSP atfı |
| `privacy-policy-en.html` | İngilizce sürüm |
| `README.md` | Bu talimatlar |

## Uygulama içi bağlantı (isteğe bağlı)

Kaynak kodda `MiaUrls.PRIVACY_POLICY` şu an `https://mialauncher.com/privacy_policy` adresine işaret ediyor. Play için GitHub URL’sini kullanacaksanız `lawnchair/src/com/mialauncher/com/MiaUrls.kt` içinde bu sabiti güncelleyebilirsiniz.
