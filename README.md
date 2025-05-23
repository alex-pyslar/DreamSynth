# DreamSynth

## Обзор
**DreamSynth** — это приложение на C# для синтеза звука и редактирования MIDI-композиций с визуализацией аудиосигналов в реальном времени. Оно предоставляет инструменты для создания и настройки звуковых волн, редактирования нот и анализа сигналов, что делает его полезным для композиторов, звуковых дизайнеров и исследователей. Построено с использованием WPF, NAudio и OxyPlot для современного интерфейса и высокой производительности.

## Особенности
- **Генератор сигналов**: Создание синусоидальных, прямоугольных и треугольных волн с настройкой частоты и амплитуды (NAudio).
- **MIDI-редактор**: Интерактивный интерфейс для создания, редактирования и воспроизведения нот с временной шкалой.
- **Визуализация сигналов**: Отображение аудиоданных в реальном времени с помощью графиков (OxyPlot).
- **Настройка темпа**: Регулировка BPM через слайдер для синхронизации воспроизведения.
- **Многопоточная обработка**: Оптимизированное воспроизведение звука с минимальными задержками.
- **Интуитивный интерфейс**: Построен на WPF с использованием XAML для удобного взаимодействия.

## Требования
- **ОС**: Windows 10 или новее.
- **IDE**: Visual Studio 2022 с поддержкой .NET 4.7.2.
- **NuGet-пакеты**:
    - NAudio (`2.2.1`) — для работы со звуком.
    - OxyPlot (`2.1.2`) — для визуализации графиков.
    - MathNet.Numerics (`5.0.0`) — для математических вычислений.
    - Microsoft.Win32.Registry (`4.7.0`) — для работы с реестром.
    - System.Security.Principal.Windows (`4.7.0`) — для управления доступом.
    - System.ValueTuple (`4.4.0`) — для поддержки кортежей.

## Установка
1. **Клонируйте репозиторий**:
   ```bash
   git clone https://github.com/alex-pyslar/DreamSynth.git
   ```
2. **Откройте проект**:
    - Запустите Visual Studio 2022.
    - Откройте файл `DreamSynth.csproj`.
3. **Восстановите NuGet-пакеты**:
    - Перейдите в `Tools > NuGet Package Manager > Restore NuGet Packages`.
4. **Соберите проект**:
    - Выберите `Build > Build Solution`.

## Запуск
1. Убедитесь, что аудиоустройство подключено и настроено.
2. Запустите приложение через Visual Studio (`F5`) или из папки `bin\Debug\DreamSynth.exe`.
3. Используйте интерфейс для:
    - Создания нот в MIDI-редакторе.
    - Настройки параметров волн в генераторе сигналов.
    - Визуализации сигналов в окне графика.
    - Управления воспроизведением с помощью кнопок Play/Stop и слайдера BPM.

## Использование
1. **MIDI-редактор**:
    - Кликните на холсте, чтобы добавить ноту.
    - Перетаскивайте ноты для изменения времени или высоты.
    - Используйте правый клик для изменения длительности.
2. **Генератор сигналов**:
    - Настройте тип волны (синус, прямоугольник, треугольник), частоту и амплитуду.
3. **Воспроизведение**:
    - Нажмите `Play` для начала воспроизведения MIDI и сигналов.
    - Нажмите `Stop` для остановки.
    - Регулируйте BPM слайдером для изменения темпа.
4. **Визуализация**:
    - График в реальном времени показывает амплитуду сигнала.

## Известные проблемы
- **Аудиоустройства**: Возможны конфликты с ASIO-драйверами; рекомендуется проверить настройки устройства.
- **Производительность**: При большом количестве нот может наблюдаться небольшая задержка (требуется оптимизация).
- **FFT**: Анализ спектра не реализован (планируется в будущих версиях).

## Будущие улучшения
- Реализация FFT для спектрального анализа сигналов.
- Добавление экспорта композиций в MIDI или WAV.
- Поддержка дополнительных типов волн (например, пилообразная).
- Оптимизация производительности MIDI-редактора для больших композиций.
- Добавление звуковых эффектов (фильтры, модуляция).

## Лицензия
Проект распространяется под лицензией Apache. Подробности см. в файле `LICENSE`.

## Контакты
Для вопросов или предложений:
- **Email**: alexpyslar@gmail.com
- **GitHub**: github.com/alex-pyslar

---
*Создано с ❤️ для музыкальных экспериментов и звукового дизайна*