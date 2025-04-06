# FeatureCollection of power plants in Belgium.
fc = ee.FeatureCollection('WRI/GPPD/power_plants').filter(
    'country_lg == "Belgium"')

# Select a single property.
single_prop = fc.select('fuel1')
print('Single property selected:', single_prop.first().getInfo())

# Select multiple properties.
multi_prop = fc.select(['fuel1', 'capacitymw'])
print('Multiple properties selected:', multi_prop.first().getInfo())

# Select multiple properties and rename them.
multi_prop_rename = fc.select(**{
    'propertySelectors': ['fuel1', 'capacitymw'],
    'newProperties': ['Fuel_1', 'Capacity_MW']
    })
print('Multiple properties selected, renamed:',
      multi_prop_rename.first().getInfo())

# Select multiple properties, remove geometry.
multi_prop_no_geom = fc.select(**{
    'propertySelectors': ['fuel1', 'capacitymw'],
    'retainGeometry': False
    })
print('Multiple properties selected, geometry removed:',
      multi_prop_no_geom.first().getInfo())https://github.com/Rucellmai61/Rucellmai61.git```json
{"recipe": {"name": "Roasted Potatoes with Chanterelles", "ingredients": ["1.5 lbs potatoes, peeled and quartered", "1 lb Chanterelles, cleaned", "1/4 cup olive oil", "1/4 cup chopped fresh parsley", "Salt and pepper to taste"], "instructions": ["Preheat oven to 400 degrees F (200 degrees C).", "In a large bowl, toss potatoes with olive oil, salt, and pepper.", "Spread potatoes in a single layer on a baking sheet.", "Roast in preheated oven for 20-25 minutes, or until potatoes are tender and golden brown.", "Add chanterelles to the baking sheet and roast for an additional 5-7 minutes, or until tender.", "Stir in parsley and serve immediately."], "notes": "You can use any type of potatoes for this recipe. I prefer to use Yukon Gold or russet potatoes. If you don't have chanterelles, you can use any other type of mushrooms.", "serving_size": "4 servings"}}

``````json
{"recipe": {"name": "Roasted Potatoes with Chanterelles", "ingredients": ["1.5 lbs potatoes, peeled and quartered", "1 lb Chanterelles, cleaned", "1/4 cup olive oil", "1/4 cup chopped fresh parsley", "Salt and pepper to taste"], "instructions": ["Preheat oven to 400 degrees F (200 degrees C).", "In a large bowl, toss potatoes with olive oil, salt, and pepper.", "Spread potatoes in a single layer on a baking sheet.", "Roast in preheated oven for 20-25 minutes, or until potatoes are tender and golden brown.", "Add chanterelles to the baking sheet and roast for an additional 5-7 minutes, or until tender.", "Stir in parsley and serve immediately."], "notes": "You can use any type of potatoes for this recipe. I prefer to use Yukon Gold or russet potatoes. If you don't have chanterelles, you can use any other type of mushrooms.", "serving_size": "4 servings"}}

```Europe</title>
<department/>1+👋 Hi, I’m @Rucellmai61
2+👀 I’m interested in ...
3+🌱 I’m currently learning ...
4+💞️ I’m looking to collaborate on ...
5+📫 How to reach me ...
6+😄 Pronouns: ...
7+⚡ Fun fact: ...

<!---
Rucellmai61/Rucellmai61 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
