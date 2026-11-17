# Actual Keyboard Mapper | نقشه‌یاب کیبورد

A trilingual on-screen keyboard drawn on a real photo of a laptop keyboard.
It does not assume a layout: it **learns what each physical key actually types** in Turkish, English and Persian, and remembers it.

یک کیبورد روی عکس واقعی کیبورد لپ‌تاپ، که چیدمان فرضی ندارد و می‌آموزد هر کلید فیزیکی واقعاً چه کاراکتری می‌فرستد.

## Features | ویژگی‌ها

- **Real keyboard photo** as the base, with a transparent overlay positioned over every key.
- **Three profiles:** Turkish (Turkish Q), English (US) and Persian, each stored separately.
- **Four states per key:** Normal, Shift, Caps Lock and AltGr.
- **View mode:** shows the learned characters; click Shift, Caps or AltGr on the image (or the state buttons) to see that layer.
- **Learn mode:** pick a state, press a physical key, and the character it produces is recorded.
- **Live feedback:** progress counter, "saved" indicator and a status line showing the last physical key pressed and the character it sent.
- **Persistent:** learned data survives closing and reopening the page.
- Single self-contained `index.html` (the image is embedded), no dependencies.

## Usage | نحوهٔ استفاده

1. Open `index.html` in your own browser (not an embedded preview, or saving may not work).
2. Set the **operating system** keyboard layout to match the profile you want to record (for example Turkish Q).
3. Choose the matching tab and switch to **Learn** mode.
4. Choose a state (Normal / Shift / Caps Lock / AltGr), then press the physical key. Repeat for each key and state.
5. Switch to **View** mode to see the learned layout.

## Important limitation | محدودیت مهم

A web page cannot change the Windows keyboard language; this is a browser security restriction. The tabs only choose which dataset you view or record. Switch the real layout yourself (usually Alt+Shift or Win+Space) and check the "last physical key" line to confirm what the keyboard really sends.

## Storage | ذخیره‌سازی

Learned data is saved per profile in the browser's `localStorage` (keys start with `kb_mapper_`). It stays in that browser, on that address. If the page shows a storage warning, open the file directly in a regular browser window.

## Author

Motasem Sadeghi

## License

[MIT](LICENSE)
