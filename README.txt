ПАМ'ЯТЬ ЗОНИ — як увімкнути акаунти й обмін (робиться один раз, ~15 хвилин)

1. Відкрий https://console.firebase.google.com і увійди своїм Google.
2. «Створити проєкт» (Create project), назва, наприклад, pamyat-zony. Google Analytics можна вимкнути.
3. Ліворуч Build → Authentication → Get started → вкладка Sign-in method → Google → Enable → Save.
4. Там же Authentication → Settings → Authorized domains → Add domain →
   впиши адресу свого сайту з Vercel, наприклад pamyat-zony.vercel.app
5. Build → Firestore Database → Create database → Production mode → регіон eur3 (Europe) → Create.
6. У Firestore відкрий вкладку Rules, видали все й встав вміст файлу firestore.rules → Publish.
7. Шестерня ⚙ біля Project Overview → Project settings → внизу «Your apps» → значок </> (Web) →
   назва будь-яка → Register app. З'явиться блок firebaseConfig = { apiKey: ... }.
8. config.js уже заповнено ключами проєкту pamyat-zony-almanakh.
9. Завантаж оновлені файли на GitHub (Add file → Upload files → Commit). Vercel сам оновить сайт за хвилину.

Твоя колекція: один раз відкрий сайт з адресою .../#import-author і увійди — колекцію автора
перенесе у твій акаунт. Далі просто заходь як звичайно.

Ключі з config.js не секретні: їх і так видно в браузері, захищає дані файл firestore.rules.
