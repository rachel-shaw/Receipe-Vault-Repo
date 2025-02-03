---
cssclasses:
  - cards
  - cards-cover
  - table-max
  - cards-cols-4
banner: "![[lunch banner.jpeg]]"
banner_y: 0.732
---
# Lunch & Dinner Menu

Take a look at this wide range of delicious, balanced meals that are perfect for any time of day. Whether you're looking for quick and easy options to fit into a busy schedule or more elaborate dishes for a special occasion, this collection has something for everyone. From hearty entrees to lighter fare, each recipe is crafted to provide both flavor and nutrition, ensuring that every meal is satisfying and enjoyable. With a variety of ingredients and cooking techniques, these recipes will inspire creativity in the kitchen while making mealtime both delicious and fulfilling.

There are `$= dv.pages("#lunchdinner_recipe").length` lunch & dinner recipes available below:
```dataview
table without id
	embed(link(cover)),
	file.link as Title,
	"**Difficulty:** " + difficulty as Difficulty,
	"**Prep time:** " + prepTime as "Prep Time",
	"**Cook time:** " + cookTime as "Cook Time",
	"**Rating:** " + rating as "Rating",
	"**Calories:** " + calories as "Calories"
FROM #lunchdinner_recipe and -"Templates"
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
 
