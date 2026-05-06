# Avenir Research & Publication

## Deploy
1. Extract ZIP → folder `Avenir_Research/`
2. Push ke GitHub
3. Connect ke Vercel (auto-detect static site)
4. Setelah dapat domain Vercel, set di Supabase Dashboard → Authentication → URL Configuration:
   - Site URL: `https://[project].vercel.app`
   - Redirect URLs: `https://[project].vercel.app/*`

## Catatan
- Tiap file HTML self-contained (CSS, JS, gambar inline)
- Auth flow butuh deployed (Supabase tidak bekerja di file://)
- DEWA & PART card belum punya cover image
