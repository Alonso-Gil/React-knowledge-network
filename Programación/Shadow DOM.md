# Usando shadow DOM
El Shadow DOM permite adjuntar arboles DOM ocultos a elemenetos en el arbol DOM regular, este arbol shadow DOM comienza con un elemento **shadow root**, debajo del cual se puede adjuntar cualquier elemento que desee, de la misna manera que el DOM normal.

Hay algunos conceptos de Shadow DOM que deben ser tomados en cuenta:
- **Shadow host**: El nodo regular del DOM al que es atado el shadow DOM.
- **Shadow tree**: El arbol DOM dentro del shadow DOM.
- **Shadow boundary**: El punto en el que el shadow DOM termina y el DOM regular comienza.
- **Shadow root**: El nodo raiz del arbol Shadow.

### ¿Que hace el shadow DOM?
Puede manipular los nodos del 'shadow DOM' de la misma manera que los nodos del arbol DOM regular. La diferencia es que nada del código dentro de un 'shadow DOM' puede afectar a nada fuera de él, lo que permite una encapsulación práctica.

---

## Referencias 
[MDN Web Docs - Usando shadow DOM](https://developer.mozilla.org/es/docs/Web/Web_Components/Using_shadow_DOM)

