---
description: Tampilkan tabel checklist progress portfolio test case Saucedemo
---

Ketika user mengetik "fitur check", tampilkan tabel berikut beserta status terbaru berdasarkan isi file test yang ada di folder `tests/`.

Cek file-file berikut untuk menentukan status ✅ atau ⬜:
- `tests/Login.spec.js`
- `tests/Homepage.spec.js`
- `tests/Cart.spec.js`
- `tests/Checkout.spec.js`

Lalu tampilkan tabel ini dengan status yang diperbarui:

---

## 📋 Progress Portfolio Test Case Saucedemo

### 🔐 `Login.spec.js`
| No | Test Case | Status |
|----|-----------|--------|
| 1  | Login valid (standard_user) | |
| 2  | Login user terkunci (locked_out_user) | |
| 3  | Login password salah | |
| 4  | Login username salah | |
| 5  | Login field kosong | |

### 🏠 `Homepage.spec.js`
| No | Test Case | Status |
|----|-----------|--------|
| 1  | Verifikasi title homepage ("Products") | |
| 2  | Verifikasi 6 produk tampil | |
| 3  | Filter nama A → Z | |
| 4  | Filter nama Z → A | |
| 5  | Filter harga Low → High | |
| 6  | Filter harga High → Low | |
| 7  | Add to cart → badge counter +1 | |
| 8  | Remove dari homepage → badge hilang | |

### 🛒 `Cart.spec.js`
| No | Test Case | Status |
|----|-----------|--------|
| 1  | Tambah 1 produk → cek muncul di cart | |
| 2  | Tambah beberapa produk → cek semua tampil | |
| 3  | Remove produk dari halaman cart | |
| 4  | Tombol "Continue Shopping" kembali ke homepage | |

### 💳 `Checkout.spec.js`
| No | Test Case | Status |
|----|-----------|--------|
| 1  | Checkout berhasil (isi semua field) | |
| 2  | Checkout tanpa First Name → error | |
| 3  | Checkout tanpa Last Name → error | |
| 4  | Checkout tanpa Zip Code → error | |
| 5  | Klik Finish → tampil halaman "Thank you" | |
