# CSS Grid
## Ejemplos y snippets útiles
### Layout de contenido y sidebar responsive
Cuando se quiere hacer un layout con grid que tenga una columna con un side-menu o una side-card y otra columna con el contenido principal, sin que ambas columnas tengan la misma altura, con el uso de `grid-template-areas` se puede conseguir esto fácilmente.
```css
.grid {
	display: grid;	
	grid-template-areas: "product card"	
						 "product .";	
	gap: 30px;	
	grid-template-columns: 2fr 1fr;
}
@media (max-width: 768px) {
	.grid {	
		grid-template-areas: "card"		
							 "product";		
		grid-template-columns: 1fr;	
	}
}
.product {
	height: 800px;	
	grid-area: product;
} 
.side-card {
	grid-area: card;	
	height: 300px;
}
```

![](grid2.gif)

### Columnas automáticas con grid
Una cuadrícula responsiva, en la que se puede establecer un tamaño mínimo que debe tener cada grid item antes de que se establezcan automáticamente las columnas para que siempre se vean bien los grid items.
```css
.grid-even-columns {
	display: grid;	
	gap: 20px;	
	grid-template-columns: repeat(auto-fit, minmax(min(300px, 100%), 1fr));
}
```

![](grid1.gif)

Poner más