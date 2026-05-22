# josm-trees-ua
JOSM Preset for mapping European trees and shrubs in Ukraine on OpenStreetMap
### v1.2
[Дерева в OpenStreetMap](https://wiki.openstreetmap.org/wiki/Uk:Tag:natural%3Dtree)

## Features
- 70+ tree species common in Ukraine (oak, chestnut, maple, sakura, linden, magnolia, thuja, etc.)
- 50+ shrub species (viburnum, juniper, lilac, rose, etc.)
- Bilingual interface (Ukrainian + English)
- Taxonomy support: species, family (taxon), leaf type and cycle
- Flower colour for ornamental trees
- Survey date and reference number for inventory work
- Heritage protection flag for natural monuments
- Tree row and hedge presets (way type)

## Можливості
- Понад 70 видів дерев, поширених в Україні (дуб, каштан, клен, сакура, липа, магнолія, туя тощо)
- Понад 50 видів кущів (калина, ялівець, бузок, шипшина тощо)
- Двомовний інтерфейс (українська + англійська)
- Підтримка таксономії: вид, родина (taxon), тип і цикл листя
- Колір цвітіння для декоративних дерев
- Дата обстеження та інвентарний номер для облікових робіт
- Прапорець охорони для пам'яток природи
- Заготовки для рядів дерев та живих огорож (тип way)

## What's new in v1.2 / Що нового у v1.2
- **Trees**: Added *Alnus glutinosa*, *Ulmus laevis*, *Pinus nigra subsp. pallasiana*, *Quercus pubescens*, *Morus* (alba/nigra), *Gleditsia triacanthos*, *Stryphnodendron excelsum*, *Sophora japonica*, *Paulownia tomentosa*. Fixed "Берізка" to "Береза" and "Рябина" to "Горобина". Updated "Дуб черешчатий" to "Дуб звичайний".
- **Shrubs**: Added *Corylus avellana*, *Frangula alnus*, *Rhamnus cathartica*, *Physocarpus opulifolius*, *Potentilla fruticosa*, *Kerria japonica*, *Vaccinium corymbosum*, *Rubus fruticosus*, *Hippophae rhamnoides*.
- **Taxonomy**: Added new families (*Adoxaceae*, *Elaeagnaceae*, *Paulowniaceae*, etc.) to the `taxon` field.
- **Дерева**: Додано *Вільху чорну*, *В'яз гладенький*, *Сосну кримську*, *Дуб пухнастий*, *Шовковицю (білу/чорну)*, *Гледичію*, *Сумах оленерогий*, *Софору японську*, *Павловнію*. Русизм «Рябина» виправлено на «Горобина», «Берізка» на «Береза». Назву «Дуб черешчатий» змінено на більш уживану «Дуб звичайний».
- **Кущі**: Додано *Ліщину*, *Крушину ламку*, *Жостір*, *Пухироплідник*, *Перстач кущовий*, *Керію*, *Лохину високорослу*, *Ожину*, *Обліпиху*.
- **Таксономія**: Розширено список родин у полі `taxon` (*Шовковицеві*, *Павловнієві*, *Лохові*, *Жостерові* тощо).

## TODO / Заплановано
0. Add icons for each species / Додати іконки для кожного виду.
1. Add quick presets for top species with auto-fill of `species:uk`, `species:en`, `taxon` / Додати швидкі заготовки для топових видів з автозаповненням.

## Howto Install JOSM Presets
**What should be done before installation in the testing mode** -> [Wiki](https://github.com/gontsa/josm-trees-ua/wiki)

Add `https://raw.githubusercontent.com/gontsa/josm-trees-ua/master/ukraine_trees.xml` in JOSM editor.

**Uk**: *Заготовки* -> *Preset preferences* -> *Активні заготовки* «+»
**En**: *Presets* -> *Preset preferences* -> *Active presets* «+»

## Howto Install Vespucci Preset
Add `https://raw.githubusercontent.com/gontsa/josm-trees-ua/master/ukraine_trees.xml` in Vespucci editor.

**Uk**: *Керування заготовками* -> *Додати заготовку* -> Вставити URL та назву заготовки
**En**: *Managing presets* -> *Add preset* -> *Active presets* «+» Paste URL for the file containing the preset and a name

⚠️ **Important Note for Vespucci Users / Важливе зауваження для користувачів Vespucci:**
- **Uk**: Щоб цей пресет коректно підтягувався для точок (`natural=tree` та `natural=shrub`), у налаштуваннях Vespucci необхідно **вимкнути стандартний (дефолтний) пресет**, інакше застосовуватимуться вбудовані базові теги редактора. (*Налаштування* -> *Інструменти мапінгу* -> *Заготовки тегів* -> Вимкнути *Вбудовані заготовки*).
- **En**: For this preset to work correctly for nodes (`natural=tree` and `natural=shrub`), you must **disable the default preset** in Vespucci settings. Otherwise, the editor's built-in basic tags will override it. (*Preferences* -> *Mapping tools* -> *Tag presets* -> Uncheck *Built-in presets*).

## Tags used
| Key | Values | Description |
|---|---|---|
| `natural` | `tree`, `shrub`, `tree_row` | Object type |
| `barrier` | `hedge` | For living fences |
| `species` | Latin name | e.g. `Quercus robur` |
| `species:uk` | Ukrainian name | e.g. `Дуб звичайний` |
| `species:en` | English name | e.g. `English Oak` |
| `taxon` | Family | e.g. `Fagaceae`, `Rosaceae` |
| `leaf_type` | `broadleaved`, `needleleaved` | |
| `leaf_cycle` | `deciduous`, `evergreen` | |
| `flower:colour` | `white`, `pink`, `red`, etc. | British spelling |
| `height` | metres | |
| `diameter_crown` | metres | |
| `circumference` | metres | Trunk circumference |
| `denotation` | `urban`, `avenue`, `landmark`, `natural_monument` | |
| `condition` | `healthy`, `damaged`, `diseased`, `dead` | |
| `age_class` | `young`, `mature`, `old` | |
| `protected` | `yes` | Heritage / natural monument |
| `survey:date` | YYYY-MM-DD | Date of field survey |
| `description:uk` | text | Free description in Ukrainian |
| `ref` | text | Inventory number |

## License
GPL v2 — same as JOSM defaultpresets.
