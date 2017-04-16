Exercise Angular 3


1. What is Component decorator in Angular 2?
	```js  s the component metatdata

	selector - css selector that identifies this component in a template
	styleUrls - list of urls to stylesheets to be applied to this component's view
	styles - inline-defined styles to be applied to this component's view
	template - inline-defined template for the view
	
	What does @Component decorator do?

	```js Marks a class as an Angular component and collects component configuration metadata.

2. What is @Directive decorator in Angular 2?
	```js change the structure of the view
	What does @Directive decorator do?
	```js exportAs - name under which the component instance is exported in a template
	```js host - map of class property to host element bindings for events, properties and attributes
	```js inputs - list of class property names to data-bind as component inputs
	```js outputs - list of class property names that expose output events that others can subscribe to
	```js providers - list of providers available to this component and its children
	```js queries - configure queries that can be injected into the component
	```js selector - css selector that identifies this component in a template

Summary
	1. Explain @Input decorator in Angular 2?
		```js @Input is used to define an input property to achieve component property binding
	2. Explain @Output decorator in Angular 2?
		```js @Output is used to define output property to achieve custom event binding.
	3. component  is also a type of directive with template,styles and logic part
	directive like *ngFor and *ngIf used for changes the DOM layout by adding and removing DOM elements. 

	```js  import {Component} from '@angular/core';

@Component({
    selector : 'my-app',
    template : `
    <h2>Exercise </h2>
    <input type="text" [(ngModel)] = "name" />
    <p>{{angular}} hello {{name}}</p>
    `,

	})
 	export class Component {

    public angular = 'Angular 2';
 	}

