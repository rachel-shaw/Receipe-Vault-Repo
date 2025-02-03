---
banner: "![[snack2.jpeg]]"
banner_y: 0.384
cssclasses:
  - cards
  - cards-cover
  - table-max
  - cards-cols-4
---
# Snack & Side Dishes

The snack and side dish section of this cookbook features a variety of tasty and versatile options perfect for any meal or occasion. Whether you're looking for something quick and light to nibble on, or a flavorful side to complement a main course, this collection has something to satisfy every craving. From savory bites to lighter, healthier choices, these recipes are designed to be both delicious and easy to prepare, making them ideal for any time of day.

# Snack Menu

There are `$= dv.pages("#snack_recipe").length` snack recipes available below:
```dataview
table without id
	embed(link(cover)),
	file.link as Title,
	"**Difficulty:** " + difficulty as Difficulty,
	"**Prep time:** " + prepTime as "Prep Time",
	"**Cook time:** " + cookTime as "Cook Time",
	"**Rating:** " + rating as "Rating",
	"**Calories:** " + calories as "Calories"
FROM #snack_recipe and -"Templates"
SORT file.name ASC
```

# Side Dish Menu

There are `$= dv.pages("#side_dish").length` side dish recipes available below:
```dataview
table without id
	embed(link(cover)),
	file.link as Title,
	"**Difficulty:** " + difficulty as Difficulty,
	"**Prep time:** " + prepTime as "Prep Time",
	"**Cook time:** " + cookTime as "Cook Time",
	"**Rating:** " + rating as "Rating",
	"**Calories:** " + calories as "Calories"
FROM #side_dish and -"Templates"
SORT file.name ASC
```

# Quick Add-Ons

```ccard
style: card
col: 2

items: [
    {
        title: 'Veggies',
        link: 'Table of Contents/Other Categories/Quick Veggies.md',
        image: 'Images/veggiebanner.jpg',
        brief: '',
        foot: ' recipes'
    },
    {
        title: 'Fruits',
        link: 'Table of Contents/Other Categories/Quick Fruits.md',
        image: 'Images/fruit banner3.jpeg',
        brief: '',
        foot: ' recipes'
    },
    {
        title: 'Starchy Carbs',
        link: 'Table of Contents/Other Categories/Quick Starchy Carbs.md',
        image: 'Images/pasta banner2.jpeg',
        brief: '',
        foot: ' recipes'
    }
]

```





```meta-bind-button
label: Back to Main Menu
icon: "book-open-check"
hidden: false
class: navigation-buttons-center
tooltip: ""
id: menu-button
style: primary
actions:
  - type: open
    link: "[[Menu]]"

```
 


