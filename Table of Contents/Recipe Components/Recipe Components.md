---
cssclasses:
  - cards
  - cards-cover
  - table-max
  - cards-cols-4
---

# Recipe Components

Building the foundation of a great meal starts with mastering the basics, like doughs, sauces, and other essential bases. These components are the starting point for creating a wide variety of dishes, from hearty pizzas to savory pastas and flavorful pastries. By understanding the techniques and ingredients that go into these foundational elements, you'll be able to build on them to create endless variations and elevate your cooking. Whether it's a simple dough for bread or a rich sauce for pasta, these basics will provide the backbone for many of your favorite meals.

There are `$= dv.pages("#recipe_components").length`  recipes components available below:
```dataview
table without id
	embed(link(cover)),
	file.link as Title,
	"**Difficulty:** " + difficulty as Difficulty,
	"**Prep time:** " + prepTime as "Prep Time",
	"**Cook time:** " + cookTime as "Cook Time",
	"**Rating:** " + rating as "Rating",
	"**Calories: **" + calories as "Calories"
FROM #recipe_components  and -"Templates"
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
 
