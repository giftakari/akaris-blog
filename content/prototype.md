---
title: "JavaScript Prototype -Godsgift Akari"
date: 2019-05-14T14:46:10+06:00
description: "JavaScript prototype"
type: "post"
image: "custom_images/Gift_Akari_Profile.png"
categories:
  - "JavaScript"
tags:
  - "Web"
  - "Software"
---

### JavaScript Prototype

Let's imagine that we need to design a cars, cars have different make and functions. First we start by designing a template and then use same to make different car model.

```js
// Using JavaScript Prototype

function Car(model, energy) {
  this.model = model;
  this.energy = energy;
}

Car.prototype.cost = function(amount) {
  console.log(`${this.model} current cost.`);
  this.energy += amount;
};

Car.prototype.speed = function(length) {
  console.log(`${this.model}  speed capcity.`);
  this.energy += length;
};

const mazda = new Car("Mazda", 3000);
```

We've designed the template of our Car that we can use to build other cars we only need to change a few things from the tempate. Let's say we we want to make Mazda, Toyota etc model. All we need is to make modify the template.

```js
// Our Toyota Model of the Car
function Toyota(model, energy, speed) {
  this.model = model;
  this.energy = energy;
  this.speed = speed;
}

Toyota.prototype.cost = function(amount) {
  console.log(`${this.model} current value.`);
  this.energy += amount;
};

Car.prototype.speed = function() {
  console.log(`Speed in KM`);
  this.speed += 1;
};

//We've addded a speed method to Totayo
```

We've created a Toyota class and added another method to Totayo.
