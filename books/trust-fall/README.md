# trust-fall

> Bu kitabın **hub klasörü**. Kitaba dair her şey (config, meta, prompt, upload pack) burada; render çıktıları `public/` ve `out/` altında, aşağıda linkli.

## Dosyalar

| | Konum | Not |
|---|---|---|
| 🎬 Final video | `out/trust-fall.mp4` _(yok)_ | render çıktısı |
| 🖼️ Thumbnail | `out/thumbnail-trust-fall.png` _(yok)_ | YouTube kapak |
| 📝 YouTube pack | `books/trust-fall/youtube.md` _(yok)_ | başlık/açıklama/tag/bölümler |
| 💬 Captions (CC) | `public/captions/trust-fall.clean.vtt` _(yok)_ | YouTube'a "With timing" yükle |
| 💬 Captions (ham) | [`public/captions/trust-fall.vtt`](../../public/captions/trust-fall.vtt) | kelime-zamanlı (karaoke kaynağı) |
| 🎙️ Audio | `public/audio/trust-fall.m4a` _(yok)_ | NotebookLM sesi |
| 🖼️ Scene images | `public/scenes/trust-fall/` _(yok)_ | Flux görselleri |
| ✍️ NotebookLM prompt | [`books/trust-fall/prompt.notebooklm.md`](prompt.notebooklm.md) | orijinal analiz açısı |
| 📖 Manifest | [`books/trust-fall/book.json`](book.json) | book.json (slug/başlık/engine) |
| ⚙️ Vox config | `books/trust-fall/config.vox.json` _(yok)_ | render config (beats/captions) |
| ⚙️ YouTube meta | `books/trust-fall/youtube-meta.json` _(yok)_ | SEO/meta + thumbnail brief |
| 🎞️ Render chunks | `out_Vox-trust-fall_chunks/` _(yok)_ | ara mp4 parçaları + parts.txt |

## Yükleme sırası
1. `out/trust-fall.mp4` yükle
2. Başlık + açıklama (bölümler tıklanabilir olur) + tag → [youtube.md](youtube.md)
3. Thumbnail → `out/thumbnail-trust-fall.png`
4. CC → `trust-fall.clean.vtt` ("With timing")
5. **Altered content = Yes** (sentetik ses)

## Yeniden üretmek
```bash
node scripts/make-book.js --slug=trust-fall --title="trust-fall"
```
