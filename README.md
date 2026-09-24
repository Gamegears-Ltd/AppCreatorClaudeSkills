<!-- сгенерировано scripts/gen-marketplace.mjs из skills/ репозитория App Creator — правки здесь затрутся -->
# Скиллы GameGears для Claude Code

Навыки, которые учат Клода работать с конвейером GameGears: сдавать прототипы в Google Play,
подключать к ним аналитику и следить за статусом сдачи. Скилл не пересказывает требования — он читает
их живыми со стойки, поэтому обновлять его приходится только тогда, когда меняется сам способ работы.

## Установка

```bash
claude plugin marketplace add Gamegears-Ltd/AppCreatorClaudeSkills
claude plugin install prototype-shipping@AppCreatorClaudeSkills
```

## Что внутри

### prototype-shipping · 1.0.2

Сдать прототип GameGears в Google Play и подключить к нему аналитику. Use when the user is building a GameGears prototype and says «залей в стор», «сдай игру», «подключи аналитику/события», «какие события слать», «что нужно для выкладки», «статус моей сдачи», "ship the prototype", "upload to Play", "wire up analytics events". НЕ для чужих игр и не для выпуска в Live — выпуск жмёт человек.
