# Flexbox by [Wes Bos](https://flexbox.io/) 

## Flex-direction 

* Works on containers. 

```css
   flex-direction : row; /* Default, wherein the main axis goes from left to right, cross axis from top to bottom. */
   flex-direction : column; /* Main axis goes from top to bottom. */
   flex-direction : row-reverse; 
   flex-direction : column-reverse;
```

## Flex-wrap

* Works on containers.

```css
   flex-wrap: wrap; 
```

## Flex-ordering

* Works on flex items
  1. Default order on flex items is 0.
  1. A higher order takes the item to right.
  1. A lower order takes the item to left.
  1. Negative values of order are legit.

```css
   order: SOMENUMERICALVALUE;
```

## Flex-alignment with justiy-content

* Works on containers

```css

    justify-content: flex-start; /*default*/
    justify-content: flex-end;
    justify-content: center;
    justify-content: space-between;
    justify-content: space-around;
```
#### To align vertically

```css
    min-height: 100vh; /*Givin it height > contents is necessary else the container will end as soon as items are enclosed.*/
    flex-direction: column; /*change main axis from top to bottom*/
    justify-content: center; /*now the divs are aligned vertically in the center*/
```

## Flex-alignment with align-items

* Works on containers
* Works on cross axis(!important point to notice) cos align-items:center wont work on main axis.

```css
     align-items: stretch; /*default*/
     align-items: center; /*this aligns the item across the cross axis, not the main axis, so give container some height*/
     height: 100vh; /*Without height it wont be able to center across the cross axis.*/
     align-items: flex-end;
     align-items: baseline; /*will align to the base of the text in each box*/
```
}

