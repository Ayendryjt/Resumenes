# Resumenes
#  Ayendry Jimene 2020 0692

Este documento resume los selectores CSS aplicados durante la actividad de CSS Diner.

CSS Diner es un juego interactivo diseñado para enseñar y practicar el uso de selectores CSS. Desarrollado por Flukeout, este juego presenta 32 niveles en los que los jugadores deben utilizar diferentes selectores CSS para elegir elementos en una mesa de alimentos virtual​ (KeepCoding Bootcamps)​​ (CSS Diner)​.

El juego es particularmente útil para principiantes y desarrolladores experimentados que desean mejorar o refrescar sus habilidades en CSS. A través de una serie de desafíos progresivos, los jugadores aprenden a aplicar selectores básicos y avanzados en un entorno lúdico y práctico, lo que facilita la comprensión y el dominio de estos conceptos​ (Vikinguard)​.

## Descendante Selector
```css
p strong {}

Este selector aplicará estilos a todos los elementos <strong> que se encuentran dentro de elementos <p>. Es decir, seleccionará los <strong> que son descendientes de <p>, sin importar cuántos niveles de profundidad haya entre ellos.
```
Selecciona todos los elementos dentro de un elemento.

## Class Selector
```css
apple.small {
  color: blue;
}
Este selector aplicará el color azul a todos los elementos que tengan ambas clases: apple y small.
```
Selecciona la clase usando .className, puede combinarse con los demas selectores.

## Comma Combinator

```css
a, p, .fun {
  color: blue;
}

```
Combina varios elementos con comas y se puede combinar con los demas selectores. El combinador de coma en CSS permite agrupar varios selectores para aplicarles el mismo conjunto de estilos. 

## Universal Selector
```css
*
```
Selecciona todos los elementos. se puede combinar con los demas para filtrar la seleccion

## Adjacent Sibling Selector

```css
A + B
```
Selecciona el elemento B que es hermano adyacente del elemento A. puede ser combinado con los demas selectores.

## General Sibling Selector
```css 
A ~ B
```
Selecciona todos los elementos B que son hermanos del elemento A. Es parecido al anterior pero selecciona todos en vez de solo uno.
## Type selector

```css
p {
  color: blue;
}

```
Selecciona todos los elementos de su tipo

## ID selector
```css
ul#long {}
El selector de ID en CSS se utiliza para aplicar estilos a un elemento específico que tiene un identificador único. La sintaxis básica del selector de ID usa el signo de almohadilla (#) seguido del valor del ID.
```
selecciona el element con una id especifica, puede usarse junto al type selector


## Child Selector
```css
A > B
```
Selecciona todos los elementos B que son hijos directos del elemento A. 

## Pseudo Selectors

- **`:first-child`**: Selecciona el primer hijo de un elemento padre. 
- **`:only-child`**: Selecciona el único hijo de un elemento. 
- **`:last-child`**: Selecciona el último hijo de un elemento padre.
- **`:nth-child()`**: Selecciona el N hijo de su elemento padre, sin importar el tipo de elemento. El N del hijo se especifica en el parentesis
- **`:nth-last-child()`**: Selecciona el N hijo desde el final dentro de un elemento. Cuenta los hijos desde el último hasta el primero.
- **`:first-of-type`**: Selecciona el primer elemento de un tipo dentro de su elemento padre.
- **`:nth-of-type()`**: Selecciona todos los elementos de un tipo específico que están en posiciones pares dentro de su elemento padre.

- **`:only-of-type`**: Selecciona el único elemento de un tipo dentro de su elemento padre.
- **`:last-of-type`**: Selecciona el último elemento de un tipo un elemento padre.
- **`:empty`**: Selecciona todos los elementos de un tipo que no tienen hijos ni contenido alguno.
- **`:not(.small)`**: Selecciona todos los elementos de un tipo que no tienen la clase "small". clase específica.

## Attributes Selectors

- **`[Attribute]`**: Selecciona todos los elementos que tienen el atributo `Attribute`, sin importar su valor. 
- **`plate[Attribute]`**: Selecciona todos los elementos `<plate>` que tienen el atributo `Attribute`. 
- **`[Attribute="Vitaly"]`**: Selecciona todos los elementos que tienen el atributo `Attribute` con el valor exacto "Vitaly".
- **`[Attribute^="Sa"]`**: Selecciona todos los elementos que tienen el atributo `Attribute` cuyo valor comienza con "Sa".
- **`[Attribute$="ato"]`**: Selecciona todos los elementos que tienen el atributo `Attribute` cuyo valor termina en "ato".
- **`[Attribute*="obb"]`**: Selecciona todos los elementos que tienen el atributo `Attribute` cuyo valor contiene la cadena "obb".