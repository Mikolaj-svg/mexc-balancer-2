# 📱 MEXC LP Balancer (Android)

Android-приложение на **Kotlin + Jetpack Compose**, предназначенное для мониторинга и автоматического ребалансирования LP-позиции и шортов на бирже **MEXC**.

---

## ⚙️ Возможности

✅ Получение актуальных цен с MEXC (REST API)  
✅ Чтение состояния пула Uniswap V3 через GraphQL (The Graph)  
✅ Расчёт отклонения между LP-стоимостью и шортом  
✅ Автоматическая ребалансировка при превышении порога  
✅ Работа как в **тестовом**, так и **в боевом** режиме

---

## 🧩 Стек технологий

- **Kotlin**  
- **Jetpack Compose**  
- **Retrofit + Moshi + OkHttp**  
- **Coroutines / Flow**  
- **The Graph API (Uniswap V3)**

---

## 🚀 Как запустить

### 1️⃣ Подготовь проект

- Скопируй структуру файлов в папку `mexc_lp_balancer_project/`
- Открой проект в Android Studio или собери через Gradle CLI  
  *(Android Studio не обязательна, см. ниже “Сборка без IDE”)*

---

### 2️⃣ Добавь свои API-ключи

Открой файл `app/build.gradle` и замени строки:

```gradle
buildConfigField "String", "MEXC_API_KEY", '"YOUR_API_KEY_HERE"'
buildConfigField "String", "MEXC_API_SECRET", '"YOUR_API_SECRET_HERE"'
