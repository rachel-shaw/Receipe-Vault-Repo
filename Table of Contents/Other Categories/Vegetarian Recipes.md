---
cssclasses:
  - cards
  - cards-cover
  - table-max
  - cards-cols-4
banner: "![[vegbanner.jpg]]"
banner_y: 0.512
---
# Vegetarian Recipes

 This section includes a variety of hearty and flavorful plant-based recipes perfect for lunch or dinner. From vibrant vegetable stir-fries to savory grain bowls and satisfying pasta dishes, these meals are designed to be both nutritious and delicious. Packed with fresh ingredients, healthy fats, and plant-based proteins, these recipes ensure that each meal is filling and well-balanced. Whether you're a long-time vegetarian or simply looking to add more meatless meals to your routine, these dishes offer a diverse selection that is both satisfying and easy to prepare for everyday dining.
 
There are `$= dv.pages("#vegetarian").length` vegetarian recipes available below:
```dataview
table without id
	embed(link(cover)),
	file.link as Title,
	"**Difficulty:** " + difficulty as Difficulty,
	"**Prep time:** " + prepTime as "Prep Time",
	"**Cook time:** " + cookTime as "Cook Time",
	"**Rating:** " + rating as "Rating",
	"**Calories: **" + calories as "Calories"
FROM #lunchdinner_recipe and #vegetarian and -"Templates"
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
 
