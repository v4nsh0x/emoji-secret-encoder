# 🔐 Emoji Secret Encoder

A small experiment where emojis carry hidden messages.

The idea is simple: you see normal emojis, but there's invisible data inside them.

---

## ✨ What it does

* Hide a message inside emojis
* Extract the hidden message back
* Uses zero-width Unicode characters (invisible to the eye)
* Works entirely in the browser

---

## 🧠 How it works (short version)

Your message is:

1. Converted to binary
2. Binary gets mapped to invisible characters

   * 0 → zero-width space
   * 1 → zero-width non-joiner
3. That invisible data is appended to emojis

So what you see:

```
😎🔥
```

What actually exists:

```
😎🔥 + hidden binary data
```

---

## 🚀 Try it

1. Enter any emojis (like 😎🔥💀)
2. Enter your secret message
3. Click **Encrypt**
4. Copy and send it

To decode:

* Paste the emojis
* Click **Decrypt**

---

## 📁 Project structure

```
index.html
```

No frameworks, no dependencies — just plain HTML, CSS, and JS.

---

## ⚠️ Note

This is not meant for serious encryption or security.

It's just a fun way to explore:

* Unicode tricks
* Basic encoding
* Steganography concepts

---

## 💡 Why I made this

Was playing around with zero-width characters and realized you can hide data in plain sight.
Turned it into a small tool for fun.

---

## 👨‍💻 Author

v4nsh0x

---

## 📜 License

MIT License — feel free to use, modify, or build on top of it.
