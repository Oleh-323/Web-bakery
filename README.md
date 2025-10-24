# 🌐 Web Project (HTMX + HTML + CSS)

## 📁 Структура проєкту
```r 
WEB/
│
├── index.html # Головна сторінка 
│
├── css/
│ ├── style.css # Основні стилі сторінки
│ ├── root.css # Глобальні змінні або стилі
│ └── page/ # Всі css коди для секцій 
│
├── html/ # Всі секції (по одиночно)
│
├── js/ # (поки що порожньо, для майбутніх скриптів)
│
└── resources/ # (папка для зображень, іконок та інше)
 ```

## ⚙️ Як це працює htmx?


- ### 1. **HTMX** підключається через CDN:
   ```html
   <script src="https://unpkg.com/htmx.org@1.9.9">
   </script>


- ### 2. У **index.html** є секція:
    ```html
    <section
        class="header border"
        data-hx-trigger="load"
        data-hx-swap="outerHTML"
        data-hx-get="html/header.border.html"
    ></section>
    ```
    - `data-hx-trigger="load"` - відправляє запит, одразу після прогрузки сторінки.
    - `data-hx-swap="outerHTML"` -замінює сам `<section>` на отриманим вмістом.
    - `data-hx-get="html/header.border.html"` - шлях до `HTML` файла, який загружається.


- ### 3. `HTMX` робить GET-запит:
    до `html/header.border.html` і вставляє його в `DOM` без перезавантаження сторінки.




# Figma
🌐 [Figma](https://www.figma.com/design/1TpV7a6dzNQqF1gHJuDvly/Web--Design-and-web-programs?node-id=115-6&t=t2Z3rX6DxXFAq8cW-0)

💜 [Git Page(No working😁)]()

🧐 [Git Hub](https://github.com/Oleh-323/Web-bakery)