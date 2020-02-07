# catalog

##### Weave Brand


| Field       | Type                  | Description                                       |
|-------------|-----------------------|---------------------------------------------------|
| id          | string                |                                                   |
| name        | string                |                                                   |
| logo        | string               | URL      |

##### Weave Product

| Field       | Type                  | Description                                       |
|-------------|-----------------------|---------------------------------------------------|
| name        | string                |                                                   |
| strain      | string                | ID of matching strain if that exists              |
| description | string                |                                                   |
| brand_id    | string                | ID of top level brand                                              |
| subcategory | string                | See Category Table                                |
| category    | string                | concentrate, edible, flower, merchandise, topical |
| id          | string                | UUID                                              |
| type        | string                | cannabis, hemp, other                             |
| variants    | array of Weave Variant|                                                   |
| experience  | string                | focus, unwind, sleep, energize etc                |
| effects     | Array of strings      | Sleepy, hungry, pain relief, happy, relaxed       |
| flavor      | dropdown of strings   | Example: ["pine", "lemon", "chocolate"]           |
| image       | string                | URL                                               |

##### Weave Variant

| Field     | Type                | Description                                 |
|-----------|---------------------|---------------------------------------------|
| name      | string              |                                             |
| price     | float               | Base retail price                           |
| cpc       | string              | Weave cannabis product code                 |
| type      | string              | unit, loose, shake, prepack, preroll        |
| potency   | Object compounds and mg| {thc: 100, cbd: 20, cbn: 4}              |
| count     | number              | Quantity in package                         |
| uom       | string              | ct, oz, ml, g                               |
| States    | Array of strings    | Example: ["ca", "co", "or"] or ["all"]      |
| Medical   | Bool                | Is it medical specific                      |
| image     | string              | URL                                         |

##### Category Structure

| Category    | Subcategories                                                                                                           |
|-------------|-------------------------------------------------------------------------------------------------------------------------|
| concentrate | syringe, crumble, crystalline, cured extract, shatter, tincture, resin, budder, hash, solventless, distillate, wax, kief, live extract, oil, cartridge, diamonds |
| edible      | snack, drink, cooking, capsule, tincture, candy, chocolate, baked                                                      |
| flower      | indica, sativa, clone, other, seeds, hybrid, caviar                                                                     |
| merchandise | vape, glass, accessory, clothing, misc                                                                                  |
| topical     | bath, ointment, oil, lotion, patch, salve, balm, intimate   
