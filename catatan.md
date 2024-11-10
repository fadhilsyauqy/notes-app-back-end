# Nodemon

Tools pertama adalah nodemon, ia bisa dikatakan wajib digunakan selama proses pengembangan. Pasalnya, dengan tools ini kita tak perlu menjalankan ulang server ketika terjadi perubahan pada berkas JavaScript. Nodemon akan mendeteksi perubahan kode JavaScript dan mengeksekusi ulang secara otomatis.

Untuk menggunakannya, pasanglah package nodemon pada devDependencies dengan mengeksekusi perintah berikut di Terminal proyek:

```bash
npm install nodemon --save-dev
```
---

# ESLint

Untuk menggunakan ESLint, pasanglah package ESLint pada devDependencies proyek Anda. Caranya, silakan eksekusi perintah berikut di Terminal:

```bash
npm init @eslint/config@latest
```

Kemudian, Anda akan diberikan beberapa pertanyaan. Silakan jawab pertanyaan yang ada dengan jawaban berikut:

- How would you like to use ESLint? -> To check syntax and find problems
- What type of modules does your project use? -> CommonJS (require/exports).
- Which framework did you use? -> None of these. 
- Does your project use TypeScript? -> No.
- Where does your code run? -> Node (pilih menggunakan tanda panah atau spasi di keyboard).
- Would you like to …… (seluruh pertanyaan selanjutnya) -> Y.


Di bawah ini adalah langkah-langkah untuk mengonfigurasi ESLint dengan tiga gaya penulisan JavaScript yang populer: Airbnb, Google, dan StandardJS.

## 1. Airbnb JavaScript Style Guide

Airbnb adalah salah satu gaya yang paling banyak digunakan, terutama di proyek JavaScript modern. Untuk mengonfigurasi ESLint dengan gaya Airbnb:

### Langkah-langkah:
1. Pasang ESLint dan konfigurasi Airbnb:

    ```bash
    npm install eslint eslint-config-airbnb eslint-plugin-import eslint-plugin-react --save-dev
    ```

2. Buat atau perbarui file konfigurasi ESLint (.eslintrc.json atau .eslintrc.js). Jika Anda belum memiliki file ESLint, buatlah dengan perintah:

    ```bash
    npx eslint --init
    ```

3. Setelah itu, tambahkan konfigurasi berikut di dalam file `.eslintrc.json` atau `.eslintrc.js`:

    **Contoh `.eslintrc.json`:**
    ```json
    {
      "extends": [
        "airbnb"
      ],
      "env": {
        "browser": true,
        "es2021": true
      },
      "parserOptions": {
        "ecmaVersion": 12,
        "sourceType": "module"
      }
    }
    ```

4. Jalankan ESLint untuk memeriksa kode Anda:

    ```bash
    npx eslint .
    ```

Airbnb mengatur banyak aturan, termasuk format kode, penggunaan tanda kutip, dan cara penanganan berbagai pola dalam JavaScript.



## 2. Google JavaScript Style Guide

Google memiliki aturan yang lebih ketat terkait penamaan variabel, penggunaan tanda kutip, dan lain-lain. Untuk menggunakan gaya Google dalam ESLint:

### Langkah-langkah:
1. Pasang ESLint dan konfigurasi Google:

    ```bash
    npm install eslint eslint-config-google --save-dev
    ```

2. Buat atau perbarui file konfigurasi ESLint (.eslintrc.json atau .eslintrc.js):

    **Contoh `.eslintrc.json`:**
    ```json
    {
      "extends": [
        "google"
      ],
      "env": {
        "browser": true,
        "es2021": true
      },
      "parserOptions": {
        "ecmaVersion": 12,
        "sourceType": "module"
      }
    }
    ```

3. Jalankan ESLint untuk memeriksa kode Anda:

    ```bash
    npx eslint .
    ```

Gaya Google mengutamakan keterbacaan dan konsistensi dalam penamaan variabel, serta memperhatikan hal-hal seperti pemisahan baris kode.


## 3. StandardJS JavaScript Style Guide

StandardJS adalah gaya yang lebih minimalis, dan terkenal karena tidak mengharuskan titik koma (`;`). Untuk menggunakan StandardJS dengan ESLint:

### Langkah-langkah:
1. Pasang ESLint dan konfigurasi Standard:

    ```bash
    npm install eslint eslint-config-standard eslint-plugin-import eslint-plugin-node eslint-plugin-promise --save-dev
    ```

2. Buat atau perbarui file konfigurasi ESLint (.eslintrc.json atau .eslintrc.js):

    **Contoh `.eslintrc.json`:**
    ```json
    {
      "extends": [
        "standard"
      ],
      "env": {
        "browser": true,
        "es2021": true
      },
      "parserOptions": {
        "ecmaVersion": 12,
        "sourceType": "module"
      }
    }
    ```

3. Jalankan ESLint untuk memeriksa kode Anda:

    ```bash
    npx eslint .
    ```

StandardJS mengutamakan kesederhanaan dan menghilangkan aturan-aturan yang tidak perlu, seperti titik koma, untuk membuat kode lebih bersih dan lebih mudah dibaca.

---

# Nanoid

Kriteria menyebutkan bahwa properti id merupakan string dan harus unik. Kita akan menggunakan bantuan library pihak ketiga untuk menghasilkan nilainya. nanoid merupakan salah satu library yang populer untuk menangani ini. Jadi, silakan pasang library tersebut dengan perintah berikut:

```bash
npm install nanoid@3.x.x
```
*Catatan:* Pastikan Anda memasang nanoid dengan versi 3.x.x. Karena jika menggunakan versi terbaru, nanoid tidak dapat digunakan dengan format module CommonJS.

---

# Link Frontend

```bash
http://notesapp-v1.dicodingacademy.com/
```