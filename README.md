<!-- сгенерировано scripts/gen-marketplace.mjs из skills/ репозитория App Creator — правки здесь затрутся -->
# Скиллы GameGears для Claude Code

Навыки, которые учат Клода работать с конвейером GameGears: сдавать прототипы в Google Play,
подключать к ним аналитику и следить за статусом сдачи. Скилл не пересказывает требования — он читает
их живыми со стойки, поэтому обновлять его приходится только тогда, когда меняется сам способ работы.

## Установка

```bash
claude plugin marketplace add Gamegears-Ltd/AppCreatorClaudeSkills
node -e "const fs=require('fs'),path=require('path'),p=path.join(require('os').homedir(),'.claude','settings.json');fs.mkdirSync(path.dirname(p),{recursive:true});const s=fs.existsSync(p)?JSON.parse(fs.readFileSync(p,'utf8')):{};s.extraKnownMarketplaces={...(s.extraKnownMarketplaces||{}),...{'AppCreatorClaudeSkills':{'source':{'source':'github','repo':'Gamegears-Ltd/AppCreatorClaudeSkills'},'autoUpdate':true}}};fs.writeFileSync(p,JSON.stringify(s,null,2)+'\n')"
claude plugin install prototype-shipping@AppCreatorClaudeSkills
```

Вторая строка включает авто-обновление этого маркетплейса в настройках Claude Code: новая версия
скилла приезжает сама в фоне следующей сессии. Без неё маркетплейс, добавленный руками, не
обновляется никогда.

## Что внутри

### prototype-shipping · 1.0.9

Сдать прототип GameGears в Google Play, подключив к нему аналитику ClickHouse и Meta SDK до сдачи и собрав страницу в сторе по контракту. Use when the user is building a GameGears prototype and says «залей в стор», «сдай игру», «подключи аналитику/события», «подключи Meta / Facebook SDK», «какие события слать», «что нужно для выкладки», «сделай страницу в сторе», «тексты и скриншоты для Play», «иконка / feature graphic», «настрой подпись билда», «upload-ключ / keystore», «статус моей сдачи», "ship the prototype", "upload to Play", "wire up analytics events", "add Meta SDK", "store listing", "ASO", "sign the Android build". НЕ для чужих игр и не для выпуска в Live — выпуск жмёт человек.
