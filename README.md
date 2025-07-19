# 🚀 Ultra URL – Smart iOS Shortcut for Instant Link Sharing

**Ultra URL** is a powerful and flexible iOS Shortcut that makes link sharing smarter, cleaner, and faster. Whether you're sharing a blog post, video, or article, Ultra URL:

- Accepts a URL from the Share Sheet or asks you for one
- Fetches the page title using Safari Reader
- Cleans up common HTML entities (like `&#39;` → `'`)
- Lets you add an optional custom short link slug
- Uses `is.gd` with `preview=0` for instant redirection
- Formats the result for copying to your clipboard as:

```
[Page Title]
➡️ [Shortened URL]
```

---

## ✨ Features

- Smart input handling (Share Sheet or manual entry)
- Optional custom short link (e.g. `https://is.gd/mycustomslug`)
- Page title extraction using Safari Reader
- Automatic HTML entity cleanup (`&amp;`, `&quot;`, etc.)
- Short links redirect instantly (no landing page)
- Clipboard output with optional notification

---

## 📸 Example Output

```
Apple announces iOS 26 with Liquid Glass redesign
➡️ https://is.gd/iOS26vrg
```

---

## 📥 Installation

There are 2 versions of the shortcut. The "Main" version simply creates a shortened URL using is.gd. The "Custom" version asks the user to optionally enter a "Custom Slug" for the shortened URL.

You can download the current versions here

1.0

Main: https://www.icloud.com/shortcuts/e85d8ead017840b8967d80fe67b5d1fd

Custom: https://www.icloud.com/shortcuts/9239910c045641c2b6e9c4f670eb291f

---

## 🔍 How It Works

Ultra URL uses:
- **Smart input detection**: Uses Share Sheet input or prompts for a URL
- **Custom slug support**: Prompted optionally at runtime
- **Title extraction**: `Get Article using Safari Reader`
- **HTML entity cleanup**:
  - `&#39;` → `'`
  - `&quot;` → `"`
  - `&amp;` → `&`
  - `&lt;` → `<`
  - `&gt;` → `>`
- **is.gd shortening API** with `preview=0`:
  ```
  https://is.gd/create.php?format=simple&url=[OriginalURL]&preview=0&shorturl=[CustomSlug]
  ```

---

## 🪪 License

This project is licensed under the [MIT License](LICENSE).  
You’re free to use, modify, and share it — just give proper credit.

---

## 🤝 Contributing

Got ideas? Pull requests are welcome — or fork and remix to make it your own.

---

Created by [Abid Patel](https://abidpatel.com)
