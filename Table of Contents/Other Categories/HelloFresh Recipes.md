---
cssclasses:
  - cards
  - cards-cover
  - table-max
  - cards-cols-4
banner: "![[hellofresh.png]]"
banner_y: 0.408
---
# HelloFresh Recipes

Inspired by HelloFresh, this collection of recipes offers quick, convenient, and flavorful meals that make weeknight dinners a breeze. With a focus on fresh ingredients and simple cooking techniques, these recipes are designed to bring delicious, balanced meals to your table with minimal effort. Whether you're looking for light and healthy dishes or hearty, satisfying meals, these HelloFresh-inspired recipes are perfect for busy days when you still want to enjoy homemade cooking. Easy to follow and full of vibrant flavors, these meals help take the guesswork out of dinner while ensuring a delicious result every time.

There are `$= dv.pages("#hellofresh").length` HelloFresh recipes available below:
```dataview
table without id
	embed(link(cover)),
	file.link as Title,
	"**Difficulty:** " + difficulty as Difficulty,
	"**Prep time:** " + prepTime as "Prep Time",
	"**Cook time:** " + cookTime as "Cook Time",
	"**Rating:** " + rating as "Rating",
	"**Calories:** " + calories as Calories
FROM #lunchdinner_recipe and #hellofresh and -"Templates"
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
 
