---
cssclasses:
  - cards
  - cards-cover
  - table-max
  - cards-cols-4
banner: "![[holidaybanner.jpg]]"
banner_y: 0.476
---
# Holiday Recipes

Celebrate the season with a variety of festive holiday recipes that bring warmth, joy, and delicious flavors to your gatherings. From savory dishes to sweet treats, this collection offers everything you need to create memorable meals that will delight your guests. Whether you're planning a big holiday feast or simply want to add a special touch to your celebrations, these recipes are designed to be easy to prepare and perfect for any occasion. With an emphasis on seasonal ingredients and comforting flavors, these dishes will help make your holiday season even more festive and flavorful.

There are `$= dv.pages("#holiday_recipe").length` holiday recipes available below:
```dataview
table without id
	embed(link(cover)),
	file.link as Title,
	"**Difficulty:** " + difficulty as Difficulty,
	"**Prep time:** " + prepTime as "Prep Time",
	"**Cook time:** " + cookTime as "Cook Time",
	"**Rating:** " + rating as "Rating",
	"**Calories: **" + calories as "Calories"
FROM #holiday_recipe and -"Templates"
SORT file.name ASC
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
 
