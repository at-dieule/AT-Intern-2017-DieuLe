Report day 2
1. Briefly explain Event Binding in Angular?

- It is a one-wat binding. Component listening to events on the template then update the data changes

2. Data binding is the synchronization of data between the model and view components
	Use the ng-model directive to bind data from the model to the view on HTML controls (input, select, textarea)
3. 3. Event Emitters are a powerful way to communicate between components. They allow you to pass events between components, and run functions on parent components.
 have a lifecycle as Angular creates, updates, and destroys 
4. ngOnChanges()
ngDoCheck()
ngAfterContentInit()
ngAfterContentChecked()

ngAfterViewInit()
ngAfterViewChecked()

ngOnDestroy

5. ```js
	import { Component, ElementRef, ViewChild, AfterViewInit } from '@angular/core';

@Component({
  selector: 'my-app',
  template: `
    <h1>Welcome to Angular World</h1>
    <div #abc>Hello {{ name }}</div>
  `,
})
export class AppComponent {
  name: string = 'LE Xuan Dieu';

  @ViewChild(‘abc’)
  abcDiv: ElementRef;

  ngAfterViewInit() {
    this.abcDiv.nativeElement.style.backgroundColor = 'red';
  }

