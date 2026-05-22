# josm-trees-ua
JOSM Preset for mapping European trees and shrubs in Ukraine on OpenStreetMap
### v1.2
[Дерева в OpenStreetMap](https://wiki.openstreetmap.org/wiki/Uk:Tag:natural%3Dtree)

## Features
- 70+ tree species common in Ukraine (oak, chestnut, maple, sakura, linden, magnolia, thuja, etc.)
- 50+ shrub species (viburnum, juniper, lilac, rose, etc.)
- Bilingual interface (Ukrainian + English)
- **Quick Presets**: Single-click setup for top common species (Oak, Pine, Linden, Shrub Rose, etc.) with automatic background auto-fill for `species:uk`, `species:en`, `taxon`, `leaf_type`, and `leaf_cycle`.
- Taxonomy support: species, family (taxon), leaf type and cycle
- Flower colour for ornamental trees
- Survey date and reference number for inventory work
- Heritage protection flag for natural monuments
- Tree row and hedge presets (way type)

## Можливості
- Понад 70 видів дерев, поширених в Україні (дуб, каштан, клен, сакура, липа, магнолія, туя тощо)
- Понад 50 видів кущів (калина, ялівець, бузок, шипшина тощо)
- Двомовний інтерфейс (українська + англійська)
- **Швидкі заготовки**: Клік в один дотик для найпопулярніших видів (дуб, сосна, липа, кущ бузку тощо) з автоматичним фоновим заповненням тегів `species:uk`, `species:en`, `taxon`, `leaf_type` та `leaf_cycle`.
- Підтримка таксономії: вид, родина (taxon), тип і цикл листя
- Колір цвітіння для декоративних дерев
- Дата обстеження та інвентарний номер для облікових робіт
- Прапорець охорони для пам'яток природи
- Заготовки для рядів дерев та живих огорож (тип way)


## Version History / Історія версій

### v1.3
- **En**: Implemented **Quick Presets** for top-11 most common species (Oak, Chestnut, Maple, Linden, Birch, Pine, Spruce, Guelder Rose, Lilac, Mock-orange, and Privet Hedge) with automated background tagging for standard attributes (`species:uk`, `species:en`, `taxon`, `leaf_type`, `leaf_cycle`).
- **Uk**: Реалізовано **Швидкі заготовки** для 11 найпопулярніших видів (Дуб, Каштан, Клен, Липа, Береза, Сосна, Ялина, Калина, Бузок, Чубушник та Огорожа з бирючини) з автоматичним фоновим заповненням супутніх тегів (`species:uk`, `species:en`, `taxon`, `leaf_type`, `leaf_cycle`).

### v1.2
- **En (Trees)**: Added 9 new species (*Alnus glutinosa*, *Ulmus laevis*, *Pinus nigra subsp. pallasiana*, *Quercus pubescens*, *Morus alba/nigra*, *Gleditsia triacanthos*, *Stryphnodendron excelsum*, *Sophora japonica*, *Paulownia tomentosa*). Fixed botanical names: "Берізка" -> "Береза", "Рябина" -> "Горобина". Updated "Дуб черешчатий" to "Дуб звичайний".
- **En (Shrubs)**: Added 9 new species (*Corylus avellana*, *Frangula alnus*, *Rhamnus cathartica*, *Physocarpus opulifolius*, *Potentilla fruticosa*, *Kerria japonica*, *Vaccinium corymbosum*, *Rubus fruticosus*, *Hippophae rhamnoides*). Extended `taxon` family list.
- **Uk (Дерева)**: Додано 9 нових видів (*Вільха чорна*, *В'яз гладенький*, *Сосна кримська*, *Дуб пухнастий*, *Шовковиця біла/чорна*, *Гледичія*, *Сумах оленерогий*, *Софору японська*, *Павловнія*). Виправлено термінологію: русизм «Рябина» замінено на «Горобина», «Берізка» на «Береза». Назву «Дуб черешчатий» змінено на більш уживану «Дуб звичайний».
- **Uk (Кущі)**: Додано 9 нових видів (*Ліщина*, *Крушина ламку*, *Жостір*, *Пухироплідник*, *Перстач кущовий*, *Керія*, *Лохина високоросла*, *Ожина*, *Обліпиха*). Розширено перелік родин у полі `taxon`.

### v1.1 (Base Draft)
- **En**: Initial release with core European tree and shrub species. Bilingual mapping schema setup for inventory tracking (height, circumference, health condition, and metadata).
- **Uk**: Базовий реліз, що включає основний перелік європейських дерев та кущів. Налаштовано двомовну схему мапінгу для проведення облікових та інвентаризаційних робіт (висота, обхват стовбура, стан здоров'я дерева та метадані).

## TODO / Заплановано
0. Add icons for each species / Додати іконки для кожного виду.
1. Add more shrub species (specific cultivars) / Додати більше видів кущів (конкретні сорти).


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
