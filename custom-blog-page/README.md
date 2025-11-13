# Custom Blog Page

A full-featured blog application built with vanilla JavaScript, JSON Server API, and Sass/SCSS. This project demonstrates API integration, CRUD operations, modular JavaScript architecture, and modern front-end development practices for creating a dynamic blog platform.

## 🚀 Features

- **Full CRUD Operations** - Create, read, update, and delete blog posts
- **JSON Server API** - RESTful API backend simulation for data management
- **Async/Await** - Modern asynchronous JavaScript for API calls
- **Modular Architecture** - Clean code organization with separate modules
- **Sass/SCSS** - Advanced CSS preprocessing with variables and nesting
- **Real-time Updates** - Instant UI refresh after each operation
- **Responsive Design** - Mobile-friendly interface

## 📁 Project Structure

```
custom-blog-page/
├── index.html           # Main HTML structure
├── app.js               # Main application entry point
├── blog.js              # Blog class definition
├── operation.js         # CRUD operation handlers
├── request.js           # API request module
├── ui.js                # UI manipulation module
├── db.json              # JSON Server database
├── scss/                # Sass source files
│   └── *.scss          # SCSS stylesheets
├── css/                 # Compiled CSS files
│   ├── style.css       # Compiled main stylesheet
│   └── style.css.map   # Source map for debugging
├── package.json         # NPM dependencies and scripts
├── package-lock.json    # Locked versions of dependencies
└── README.md            # Project documentation
```

## 🛠️ Technologies Used

- HTML5
- Sass/SCSS
- CSS3
- Vanilla JavaScript (ES6+)
- JSON Server
- Fetch API
- Async/Await
- ES6 Classes
- NPM
- RESTful API

## 🌐 Live Demo

Visit the repository: [web-development-starter-kit](https://github.com/mirhatfidan/web-development-starter-kit)

## 💻 Getting Started

### Prerequisites

- Node.js (v12 or higher)
- NPM or Yarn package manager
- Code editor - VS Code recommended

### Installation

1. Clone the repository:
```bash
git clone https://github.com/mirhatfidan/web-development-starter-kit.git
```

2. Navigate to the project directory:
```bash
cd web-development-starter-kit/custom-blog-page
```

3. Install dependencies:
```bash
npm install
```

4. Start JSON Server (in one terminal):
```bash
npm run server
# or
json-server --watch db.json --port 3000
```

5. Compile Sass (in another terminal):
```bash
npm run sass
# or for watch mode
npm run watch
```

6. Open `index.html` in your browser:
   - Use a local development server (Live Server in VS Code)
   - Or simply open the file in browser

## 📸 Screenshots

_A modern blog platform with full CRUD functionality and clean design._

## 🎯 Learning Objectives

This project was created to practice and demonstrate:

- **RESTful API** - Working with REST principles
- **HTTP Methods** - GET, POST, PUT/PATCH, DELETE
- **Fetch API** - Making HTTP requests
- **Async/Await** - Handling asynchronous operations
- **JSON Server** - Simulating backend API
- **CRUD Operations** - Complete data management
- **ES6 Classes** - Modern JavaScript OOP
- **Module Pattern** - Code organization
- **Sass/SCSS** - CSS preprocessing
- **Error Handling** - Try/catch blocks
- **DOM Manipulation** - Dynamic UI updates

## 🎨 What You Can Do

### 1. Create New Blog Posts
Form üzerinden yeni blog yazısı ekleyebilirsiniz. Başlık, içerik, yazar gibi bilgileri girdikten sonra POST isteği ile API'ye gönderilir ve anında listeye eklenir. Veriler `db.json` dosyasında kalıcı olarak saklanır.

### 2. View All Blog Posts
Sayfa açıldığında tüm blog yazıları otomatik olarak yüklenir. Her yazı kart formatında gösterilir ve başlık, içerik, tarih, yazar bilgilerini içerir. GET isteği ile API'den çekilir.

### 3. Edit Existing Posts
Herhangi bir yazının "Düzenle" butonuna tıklayarak içeriği güncelleyebilirsiniz. Form mevcut verilerle doldurulur, değişiklikleri yaptıktan sonra PUT/PATCH isteği ile API'ye kaydedilir.

### 4. Delete Blog Posts
Yazı üzerindeki silme butonuyla blog yazısını kaldırabilirsiniz. DELETE isteği API'ye gönderilir, veri hem görünümden hem de `db.json` dosyasından silinir.

### 5. Search & Filter
Anahtar kelimeye göre yazı arama, kategori veya yazara göre filtreleme yapabilirsiniz. Arama başlık ve içerikte çalışır.

### 6. Sort Posts
Yazıları tarihe göre (en yeni/eski), alfabetik olarak veya yazara göre sıralayabilirsiniz.

## 🔧 Module Breakdown

### 1. `blog.js` - Blog Class
Blog yazısının yapısını tanımlar. Başlık, içerik, yazar ve tarih gibi özellikleri içerir.

### 2. `request.js` - API Request Module
Tüm HTTP isteklerini yönetir. GET, POST, PUT ve DELETE metodlarını içerir. Fetch API kullanarak sunucu ile iletişim kurar.

### 3. `operation.js` - CRUD Operations
Blog ile ilgili tüm CRUD işlemlerini gerçekleştirir. Tüm yazıları getirme, yeni yazı oluşturma, güncelleme ve silme fonksiyonlarını barındırır.

### 4. `ui.js` - UI Management
Kullanıcı arayüzü güncellemelerini yönetir. Blog yazılarını ekrana yazdırma, form temizleme, bildirim gösterme ve yazıları UI'dan silme işlemlerini yapar.

### 5. `app.js` - Application Entry
Uygulamanın ana giriş noktasıdır. Tüm modülleri koordine eder, sayfa yüklendiğinde blog yazılarını çeker ve event listener'ları tanımlar.

## 📦 JSON Server Database

JSON Server, `db.json` dosyasını kullanarak RESTful API simüle eder. Dosya, blog yazılarını bir dizi içinde saklar. Her yazı id, başlık, içerik, yazar, kategori ve tarih bilgilerini içerir.

### Kullanılabilen API Endpoints
- **GET** `/blogs` - Tüm blog yazılarını getir
- **GET** `/blogs/:id` - Belirli bir yazıyı getir
- **POST** `/blogs` - Yeni blog yazısı oluştur
- **PUT** `/blogs/:id` - Yazıyı güncelle (tümünü değiştir)
- **PATCH** `/blogs/:id` - Yazıyı kısmi güncelle
- **DELETE** `/blogs/:id` - Yazıyı sil

## 🚀 Eklenebilecek Gelişmiş Özellikler

Kullanıcı girişi, yorum sistemi, beğeni/oylama, görsel yükleme, zengin metin editörü, sayfalama, kategori/etiket yönetimi, arama vurgulama, taslak sistemi, sosyal medya paylaşımı, okuma süresi hesaplama, ilgili yazılar, tarihsel arşiv, RSS feed ve karanlık mod gibi özellikler ekleyebilirsiniz.

## 🔧 NPM Komutları

- `npm install` - Bağımlılıkları yükle
- `npm run server` - JSON Server'ı başlat (port 3000)
- `npm run sass` - Sass'ı CSS'e derle
- `npm run watch` - Sass değişikliklerini izle
- `npm run build` - Production CSS oluştur

## 🎓 Proje ile Öğrenilenler

RESTful API entegrasyonu, HTTP metodları (GET, POST, PUT, DELETE), asenkron JavaScript (Promises, Async/Await), ES6 Classes ve OOP prensipleri, modüler kod yapısı, Fetch API kullanımı, error handling, CSS preprocessing (Sass/SCSS) ve modern front-end development best practices konularında deneyim kazanabilirsiniz.

## 🐛 Sorun Giderme

**JSON Server başlamıyorsa:** Global olarak yükleyin (`npm install -g json-server`) veya npx kullanın (`npx json-server --watch db.json --port 3000`).

**CORS hataları:** JSON Server CORS'u otomatik yönetir. Hata alırsanız sunucunun çalıştığından ve port numarasının doğru olduğundan emin olun.

**Değişiklikler yansımıyorsa:** Tarayıcıyı yenileyin (Ctrl+F5), konsol hatalarını kontrol edin, JSON Server'ın çalıştığını ve `db.json` dosyasındaki verileri doğrulayın.

## 🤝 Contributing

This is a learning project, but suggestions and improvements are welcome!

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is created for educational purposes.

## 👨‍💻 Author

**Mirhat Fidan**

- GitHub: [@mirhatfidan](https://github.com/mirhatfidan)

## 🙏 Acknowledgments

- Part of web development coursework - API integration project
- Thanks to all team members for their contributions
- JSON Server for easy API simulation
- Focus on modern JavaScript and API development

## 📚 Learning Resources

- [JSON Server Documentation](https://github.com/typicode/json-server)
- [Fetch API - MDN](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)
- [Async/Await - JavaScript.info](https://javascript.info/async-await)
- [RESTful API Design](https://restfulapi.net/)
- [Sass Documentation](https://sass-lang.com/documentation)

---

⭐ Star this repository if you found it helpful!

