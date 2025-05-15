# dark-mode-plain-htmlcssjs

Proyek sederhana ini menunjukkan implementasi dark mode menggunakan HTML, CSS, dan JavaScript tanpa framework tambahan.

## Konfigurasi CSS untuk Dark Mode

Berikut adalah variabel CSS yang digunakan untuk tema gelap:

```css
[data-theme="dark"] {
  --bg-color: #111827;
  --container-bg: #1f2937;
  --text-color: #ffffff;
  --border-color: #374151;
  --button-bg: #2563eb;
  --button-hover: #1d4ed8;
  --toggle-bg: #374151;
  --toggle-text: #ffffff;
}
```

## Kode JavaScript untuk Toggle Dark Mode

Berikut adalah fungsi JavaScript **`toggleDarkMode()`** yang digunakan untuk mengubah tema antara terang dan gelap:

```javascript
<script>
  function toggleDarkMode() {
    document.documentElement.setAttribute('data-theme',
      document.documentElement.getAttribute('data-theme') === 'dark' ? 'light' : 'dark'
    );
  }
</script>
```

Anda dapat memanggil fungsi ini dari elemen HTML (misalnya, tombol) untuk mengaktifkan atau menonaktifkan tema gelap.

```html
<button onclick="toggleDarkMode()">Toggle Dark Mode</button>
```
