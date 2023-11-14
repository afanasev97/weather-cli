# Консольное приложение для получения прогноза погоды

Это консольное приложение позволяет получать прогноз погоды для заданного города с использованием OpenWeather API. Вы можете использовать его в командной строке для быстрого получения информации о погоде.

## Установка

Для использования этого приложения вам потребуется Node.js. Убедитесь, что он установлен на вашем компьютере.

1. Клонируйте репозиторий:

```bash
git clone https://github.com/afanasev97/weather-cli.git
```
Установите зависимости:

  ```bash
  npm install
  ```

Создайте файл конфигурации weather-config.json:

Создайте файл weather-config.json в корневой папке проекта и заполните его следующим образом:

```json
{
  "defaultCity": "Nizhny Novgorod",
  "apiKey": "your-api-key"
}
```

Замените "Nizhny Novgorod" на ваш город по умолчанию и "your-api-key" на ваш API-ключ OpenWeather.

## Использование:
Команда node weather.js запускает приложение для получения прогноза погоды в городе, указанном в файле конфигурации.

### Дополнительные опции командной строки:
-s, --city: Указание города для получения прогноза погоды.
-t, --token: Указание API-ключа OpenWeather.
-h, --help: Отображение справочной информации.
### Примеры использования:

```bash
# Получить прогноз погоды для города из файла конфигурации
node weather.js

# Получить прогноз погоды для другого города
node weather.js -s "Moscow"

# Получить прогноз погоды с использованием другого API-ключа
node weather.js -t "new-api-key"
```
## Примечание
Если файл конфигурации weather-config.json отсутствует, приложение будет использовать город по умолчанию из скрипта и требовать указать API-ключ при запуске.

## Лицензия
Этот проект распространяется под лицензией MIT.
