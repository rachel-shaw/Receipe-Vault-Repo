---
cssclasses:
  - cards
  - cards-cover
  - table-max
  - cards-cols-4
banner: "![[pasta banner2.jpeg]]"
banner_y: 0.384
---

# Quick Starchy  Carbs

Rice
Sweet potato
Red potato
Russet potato
Naan
Tortillas
Chips
Garlic bread
Pasta
Black beans
Chickpeas
Apples
Bananas
Oranges
Grapes
Berries
Quinoa
Corn

```dataview
table without id
	embed(link(cover)),
	file.link as Title,
	"**Difficulty:** " + difficulty as Difficulty,
	"**Prep time:** " + prepTime as "Prep Time",
	"**Cook time:** " + cookTime as "Cook Time",
	"**Rating:** " + rating as "Rating",
	"**Calories: **" + calories as "Calories"
FROM #starchycarbs and -"Templates"
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
 
