---
banner: "![[breakfast banner4.jpeg]]"
banner_y: 0.628
cssclasses:
  - cards
  - cards-cover
  - table-max
  - cards-cols-4
---
# Breakfast Menu

Increasing the amount of protein in your diet even slightly, from 18 to 20 percent of your total calories for the day, can help improve the quality of food choices you make, including fewer refined grains and added sugar and more green veggies.

There are `$= dv.pages("#breakfast_recipe").length` breakfast recipes available below:
```dataview
table without id
	embed(link(cover)),
	file.link as Title,
	"**Difficulty:** " + difficulty as Difficulty,
	"**Prep time:** " + prepTime as "Prep Time",
	"**Cook time:** " + cookTime as "Cook Time",
	"**Rating:** " + rating as "Rating",
	"**Calories:** " + calories as "Calories"
FROM #breakfast_recipe and -"Templates"
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
 
