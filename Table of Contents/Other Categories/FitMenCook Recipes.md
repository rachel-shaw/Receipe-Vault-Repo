---
cssclasses:
  - cards
  - cards-cover
  - table-max
  - cards-cols-4
banner: "![[fitmencookbanner1.jpg]]"
banner_y: 0.396
---
# FitMenCook Recipes

This collection of FitMenCook-inspired recipes is designed to provide nutritious, flavorful meals that support a healthy lifestyle without sacrificing taste. Packed with fresh ingredients and balanced macros, these recipes are perfect for fueling your body while keeping meals exciting and satisfying. Whether you're looking for high-protein options, wholesome grain bowls, or creative twists on classic dishes, these FitMenCook recipes are easy to prepare and ideal for those who want to enjoy delicious, wholesome food on a daily basis. From quick meals to make ahead options, each dish is designed to help you maintain a healthy diet without compromising on flavor.

There are `$= dv.pages("#fitmencook").length` FitMenCook recipes available below:
```dataview
table without id
	embed(link(cover)),
	file.link as Title,
	"**Difficulty:** " + difficulty as Difficulty,
	"**Prep time:** " + prepTime as "Prep Time",
	"**Cook time:** " + cookTime as "Cook Time",
	"**Rating:** " + rating as "Rating",
	"**Calories: **" + calories as "Calories"
FROM #lunchdinner_recipe and #fitmencook and -"Templates"
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
 
