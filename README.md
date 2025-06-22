# ✍️ Draftly

**Draftly** to lekki, multiplatformowy edytor Markdown w stylu MS Worda z wbudowaną kontrolą wersji. Idealny do pisania notatek, dokumentacji, blogów i wszędzie tam, gdzie liczy się historia zmian.

---

## 🚀 Funkcje

- 📝 Edytor Markdown z live preview
- 🗂️ Snapshoty wersji z historią zmian
- 📄 Eksport do PDF (z użyciem Pandoc)
- 💾 Otwieranie i zapisywanie plików `.md`
- 🎨 Stylizacja jak w MS Word (nagłówki, tabele, fonty)
- 🌗 Tryb jasny / ciemny
- 🧠 Praca offline – działa lokalnie
- 🔒 Twoje pliki nigdy nie trafiają do chmury

---

## 🖥️ Technologia

- **Frontend:** Vue 3 + ToastUI Editor
- **Backend:** Tauri (Rust)
- **Wersjonowanie:** Snapshot system z lokalną historią `.history/`
- **Eksport:** `pandoc` (lokalnie)

---

## 📦 Instalacja

> Upewnij się, że masz zainstalowanego [Node.js](https://nodejs.org/) oraz [Rust + Cargo](https://tauri.app/v1/guides/getting-started/prerequisites)

```bash
npm install
npm run tauri dev
```