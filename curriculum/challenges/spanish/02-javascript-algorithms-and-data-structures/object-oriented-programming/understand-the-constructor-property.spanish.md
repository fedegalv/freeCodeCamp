---
id: 587d7daf367417b2b2512b7e
title: Understand the Constructor Property
challengeType: 1
videoUrl: ''
localeTitle: Entender la propiedad del constructor
---

## Description
<section id="description"> Hay una propiedad especial de <code>constructor</code> ubicada en las instancias de objeto <code>duck</code> y <code>beagle</code> que fueron creadas en desafíos anteriores: <blockquote> let duck = new Bird(); <br> let beagle = new Dog(); <br><br> console.log (duck.constructor === Bird); // prints true <br> console.log (beagle.constructor === Dog); // prints true </blockquote> Tenga en cuenta que la propiedad del <code>constructor</code> es una referencia a la función constructor que creó la instancia. La ventaja de la propiedad  <code>constructor</code> es que es posible verificar esta propiedad para averiguar qué tipo de objeto es. Aquí hay un ejemplo de cómo se podría usar esto: <blockquote> función joinBirdFraternity (candidate) { <br> if (candidate.constructor === Bird) { <br> return true; <br> } else { <br> return false; <br> } <br> } </blockquote> <strong>Nota</strong> <br> Ya que la propiedad <code>constructor</code> puede ser sobreescrita (lo que sera cubierto en los siguientes dos desafíos), generalmente es mejor usar el método <code>instanceof</code> para verificar el tipo de un objeto. </section>

## Instructions
<section id="instructions"> Escriba una función <code>joinDogFraternity</code> que tome un <code>candidate</code> como parámetro y, utilizando la propiedad <code>constructor</code> , devuelva <code>true</code> si el candidato es un <code>Dog</code> , de lo contrario, devuelva <code>false</code> . </section>

## Tests
<section id='tests'>

```yml
tests:
  - text: <code>joinDogFraternity</code> deberia ser definido como una función.
    testString: 'assert(typeof(joinDogFraternity) === "function", "<code>joinDogFraternity</code> deberia ser definido como una función.");'
  - text: <code>joinDogFraternity</code> debería devolver true si el <code>candidate</code> es una instancia de <code>Dog</code> .
    testString: 'assert(joinDogFraternity(new Dog("")) === true, "<code>joinDogFraternity</code> should return true if<code>candidate</code> is an instance of <code>Dog</code>.");'
  - text: <code>joinDogFraternity</code> debe usar la propiedad <code>constructor</code> .
    testString: 'assert(/\.constructor/.test(code) && !/instanceof/.test(code), "<code>joinDogFraternity</code> debe usar la propiedad <code>constructor</code> ");'

```

</section>

## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function Dog(name) {
  this.name = name;
}

// Add your code below this line
function joinDogFraternity(candidate) {

}

```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
