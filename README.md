# Comments Disabler Bot

Бот позволяет включать комментарии только в избранных постах Telegram канала. 
Программа написана мною на скорую руку, так что в коде возможно наличие лапшиобразности и бестолковсти.

> Бот писался под **Python 3.8.1**, но должен работать на **Python 3.6+**.

### Настройка и запуск бота
1. С помощью `@BotFather`, создать нового бота, закинуть его в беседу, которая привязана к каналу и назначить его администратором со всеми правами;
2. Узнать ID вашего канала с помощью `@GetMyID_BOT`;
3. Настроить файл `config.yaml`:
    + Открыть `config.yaml` любым текстовым редактором;
    + В поле `Token` ввести токен вашего бота;
    + В поле `ChannelID` ввести ID вашего Telegram-канала;
    + В поле `WiteList` через дефис определить слова, которые, при наличии в тексте поста, заставят бота оставить возможность комментирования конкретной записи.
4. Через терминал или командную строку перейти в директорию бота;
5. Установить необходиые зависимости с помощью:
    + Windows: `pip install -r requirements.txt`;
    + Linux: `pip3 install -r requirements.txt`.
6. Запустить бота:
    + Windows: `python run.py`;
    + Linux: `pyton3 run.py`.

Запущенный бот будет получать у Telegram информацию о новых постах на канале и удалять их из привязанной беседы, что отключит возможность их комментировния.