# رفع الموقع على GitHub Pages (من المتصفح)

1. أنشئ مستودعاً جديداً على GitHub.
2. فك الضغط، وارفع **محتويات** المجلد إلى جذر المستودع (Add file → Upload files)،
   بحيث يكون `.github` و`wasm-page` و`Makefile` في الجذر مباشرة.
   - المجلد `.github` مخفي؛ تأكد أنه ظهر في المستودع بعد الرفع (يحتوي `workflows/wasm-pages.yml`).
   - إن لم يرفعه المتصفح: Add file → Create new file واكتب المسار `.github/workflows/wasm-pages.yml` والصق محتواه.
3. Settings → Pages → Source = **GitHub Actions**.
4. افتح تبويب Actions وشغّل "Build WASM and publish Pages" (أو ادفع أي تعديل). الـ workflow يجلب نواة المحاكي ويبنيها تلقائياً (عدة دقائق).
5. الرابط: `https://<USER>.github.io/<REPO>/` ثم ثبّته من Chrome.
