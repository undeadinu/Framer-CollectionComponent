# Framer-CollectionComponent
Framer Module working in progress

```coffeescript
{CollectionComponent} = require 'CollectionComponent'

myCollection = new CollectionComponent
	amount: 24
	columns: 4
	gutter: 1
	cellWidth: Screen.width / 4
	cellHeight: 100
	cell: (cell) ->
		coords = cell.html = cell.coords.x + ", " + cell.coords.y
		cell.style = lineHeight: cell.height + "px", textAlign: "center"
		cell.onMouseOver -> this.html = this.name
		cell.onMouseOut -> this.html = coords
```

<img width="1142" alt="screen shot 2016-10-12 at 1 33 37 pm" src="https://cloud.githubusercontent.com/assets/1941540/19298483/8d174202-9080-11e6-90fe-c48ec95e98de.png">
