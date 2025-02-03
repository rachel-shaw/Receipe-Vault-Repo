---
cssclasses:
  - cards
  - cards-cover
  - table-max
  - cards-cols-4
banner: "![[soup.jpg]]"
banner_y: 0.424
---
# Soup Recipes

Warm up with a selection of comforting and flavorful soups, perfect for any season and ideal for cozy meals. Whether you're craving a creamy, rich soup or a light, broth-based option, these recipes are designed to satisfy and nourish. From classic favorites like tomato and chicken noodle to hearty stews and spicy chili, there's something for every taste. With easy-to-follow instructions and wholesome ingredients, these soups are a simple way to enjoy a homemade, comforting meal that will warm you up and fill you up.

There are `$= dv.pages("#soup").length` soup recipes available below:
```dataview
table without id
	embed(link(cover)),
	file.link as Title,
	"**Difficulty:** " + difficulty as Difficulty,
	"**Prep time:** " + prepTime as "Prep Time",
	"**Cook time:** " + cookTime as "Cook Time",
	"**Rating:** " + rating as "Rating",
	"**Calories: **" + calories as "Calories"
FROM #lunchdinner_recipe and #soup and -"Templates"
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
 
