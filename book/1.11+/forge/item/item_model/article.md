# JSON файл модели

За отображение предмета в руках, от третьего лица и во всех остальных состояниях отвечает JSON файл, который должен
находиться по пути `src/resources/assets/*ваш modid*/models/item/item_test.json`.

Название файла `item_test` должно совпадать с регистрационным именем предмета (см. предыдущую статью).

## Структура файла

Для начала пройдемся по тегам верхнего уровня.

### parent

```json
{
  "parent": "item/generated"
}
```

Этот тег используется для указания, какую модель предмета установить в качестве родителя. В таком случае, все неуказанные
теги будут взяты от родителя.

Например в данном случае мы устанавливаем в качестве родителя модель предмета, которая имеет название `generated.json`.
Этот файл находится по пути `assets/minecraft/models/item`. Заметьте, что данный файл находится не в папке src (там только
файлы вашего мода), а в .jar файле Minecraft.

Вполне можно указать и другого родителя:

```json
{
  "parent": "item/generated"
}
```

TODO