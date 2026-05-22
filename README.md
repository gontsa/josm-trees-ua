# josm-trees-ua
JOSM Preset for mapping European trees and shrubs in Ukraine on OpenStreetMap
### v1.1 (draft version)
[Дерева в OpenStreetMap](https://wiki.openstreetmap.org/wiki/Uk:Tag:natural%3Dtree)

## Features
- 60+ tree species common in Ukraine (oak, chestnut, maple, sakura, linden, magnolia, thuja, etc.)
- 40+ shrub species (viburnum, juniper, lilac, rose, etc.)
- Bilingual interface (Ukrainian + English)
- Taxonomy support: species, family (taxon), leaf type and cycle
- Flower colour for ornamental trees
- Survey date and reference number for inventory work
- Heritage protection flag for natural monuments
- Tree row and hedge presets (way type)

## Можливості
- Понад 60 видів дерев, поширених в Україні (дуб, каштан, клен, сакура, липа, магнолія, туя тощо)
- Понад 40 видів кущів (калина, ялівець, бузок, шипшина тощо)
- Двомовний інтерфейс (українська + англійська)
- Підтримка таксономії: вид, родина (taxon), тип і цикл листя
- Колір цвітіння для декоративних дерев
- Дата обстеження та інвентарний номер для облікових робіт
- Прапорець охорони для пам'яток природи
- Заготовки для рядів дерев та живих огорож (тип way)

## TODO
0. Add icons for each species.
1. Add quick presets for top species with auto-fill of `species:uk`, `species:en`, `taxon`.
2. Add more shrub species (specific cultivars).
3. Add Vespucci-specific compatibility tests.

## Заплановано
0. Додати іконки для кожного виду.
1. Додати швидкі заготовки для топових видів з автозаповненням `species:uk`, `species:en`, `taxon`.
2. Додати більше видів кущів (конкретні сорти).
3. Перевірити сумісність з Vespucci.

## Howto Install JOSM Presets
**What should be done before installation in the testing mode** -> [Wiki](https://github.com/gontsa/josm-trees-ua/wiki)

Add `https://raw.githubusercontent.com/gontsa/josm-trees-ua/master/ukraine_trees.xml` in JOSM editor.

**Uk**: *Заготовки* -> *Preset preferences* -> *Активні заготовки* «+»
**En**: *Presets* -> *Preset preferences* -> *Active presets* «+»

## Howto Install Vespucci Preset
Add `https://raw.githubusercontent.com/gontsa/josm-trees-ua/master/ukraine_trees.xml` in Vespucci editor.

**Uk**: *Керування заготовками* -> *Додати заготовку* -> Вставити URL та назву заготовки
**En**: *Managing presets* -> *Add preset* -> *Active presets* «+» Paste URL for the file containing the preset and a name

## Tags used
| Key | Values | Description |
|---|---|---|
| `natural` | `tree`, `shrub`, `tree_row` | Object type |
| `barrier` | `hedge` | For living fences |
| `species` | Latin name | e.g. `Quercus robur` |
| `species:uk` | Ukrainian name | e.g. `Дуб черешчатий` |
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
