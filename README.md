# Android-приложение для получения информации о погоде в городе

Это Android-приложение позволяет пользователю узнать текущую погоду в заданном городе. Используется API от [WeatherAPI](https://weatherapi.com/), который предоставляет данные о погоде, включая описание погоды и температуру.

## Функциональность
- Ввод города через поле `EditText`.
- Получение данных о погоде с помощью API при нажатии кнопки.
- Отображение описания погоды и температуры.
- Показ иконки текущей погоды.

## Используемые технологии
- **Android SDK**: Приложение разработано с использованием стандартных компонентов Android.
- **JSON**: Для обработки данных погоды, полученных с сервера.
- **Glide**: Для загрузки и отображения иконки погоды.

## Структура проекта
### Основной экран
1. **EditText (editTextCity)** - Поле для ввода названия города.
2. **Button (buttonGetWeather)** - Кнопка для отправки запроса на сервер.
3. **TextView (textViewWeatherDescription)** - Текстовое поле для отображения описания погоды.
4. **ImageView (ivWeatherIcon)** - Иконка погоды.

### Логика работы
1. Приложение проверяет наличие подключения к Интернету.
2. При нажатии кнопки "Получить погоду", если город введён, приложение отправляет запрос к API с параметром города.
3. После получения данных, приложение парсит JSON-ответ и отображает:
   - Описание погоды.
   - Температуру.
   - Иконку погоды, загруженную через Glide.


## Примечания
- Приложение требует подключения к Интернету для получения данных о погоде.
- В случае ошибок при запросе или обработке данных будет отображаться сообщение об ошибке.



