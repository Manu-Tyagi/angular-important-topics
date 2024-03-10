# Angular Important Topics


- [Angular Important Topics](#angular-important-topics)
  - [What is the difference between AngularJS and Angular](#what-is-the-difference-between-angularjs-and-angular)
  - [Key Features of Angular](#key-features-of-angular)
  - [Different Versions of Angular](#different-versions-of-angular)
  - [Why TS used in Angular](#why-ts-used-in-angular)
  - [Angular Components](#angular-components)
  - [Data Binding in Angular](#data-binding-in-angular)
  - [Angular Directives](#angular-directives)
  - [Angular Modules](#angular-modules)
  - [Angular CLI](#angular-cli)
  - [Angular Services](#angular-services)
  - [Depdency Injection in Angular](#depdency-injection-in-angular)


## What is the difference between AngularJS and Angular

* AngularJS
  * It is based on MVC architecture
  * It uses JavaScript to build the application
  * Based on controllers concept
  * No support for mobile platforms
  * Difficult to build SEO friendly application
* Angular
  * This is based on Service/Controller
  * Uses TypeScript to build the application
  * This is a component based UI approach
  * Fully supports mobile platforms
  * Ease to build SEO friendly applications


## Key Features of Angular

* Two way data binding
  * changes in model state are automatically reflected in the view and vice versa, without the need for manual DOM manipulation
* MVVM Architecture
  * follows model-view-view-model architecture pattern
  * model represents application data, view renders the user interface, view-model manages communication between the model and the view
* Depedency Injection
  * allows for the creation and injection of depedencies into component and services. making code more maintainable and scalable
* Directives
  * used to create reusable components, manipulate the DOM, add event handlers etc
* Components
  * encapsulate the application logic and UI into reusable and modular pieces
  * contains template
    * defines the view
  * contains class
    * contains the logic
* Routing
  * enables navigation between different views of an app without the need to reload the entire app
* Forms
  * Template driven
    * easy to use simpler forms
  * Reactive forms
    * more flexible, more control over validation
* HTTP Client
  * module for making ajax requests to server
  * provides features of request and response interceptions, error handling and support for observables for handling asynchronous data
* Modularity
  * promotes reusability, mantainability, scalability by separation concerns and encapsulating functionality
* Testing
  * built-in support for testing using tools like Jasmine and Karma.
  * provides utilities for writing unit tests, integration tests, and end-to-end tests, ensuring the reliability and stability of Angular application
  

## Different Versions of Angular

* Angular JS (1.x)
  * released in 2010
  * by google as js based open source frontend web framework
  * utilized two way data binding and DI etc
* Angular 2 (Sept 2016)
  * complete rewrite of angularJS, not backward compatible
  * introduced component based architecture
  * used TS as primary language
  * improvement in performance, speed and mobile support
* Angular 4 (March 2017)
  * smaller and faster
  * added features like *ngIf, *ngFor, animation package, and new HTTP client
* Angular 5 (November 2017)
  * improvement in compiler, build optimizer, and HTTP client
  * add support for PWA
* Angular 6 (May 2018)
  * introduced Angular elements
  * improved angular CLI
  * enhanced support for service worker
* Angular 7 (Oct 2018)
  * improved angular CLI, angular Material and component dev kit, drag and drop
* Angular 8 (May 2019)
  * introduces differential loading for modern JS bundles
  * improvments in angular router, lazy loading, angular CLI
* Angular 9 (Feb 2020)
  * introduced IVY as default rendering engine
  * introduced improved type checking and build errors
* Angular 10 (June 2020)
  * introduces strictier type for forms and nullish coalescing
* Angular 11 (November 2020)
  * added experimental support for webpack 5
* Angular 12 (May 2021)
* Angular 13 (November 2021)
  * introduces features like HMR - Hot module replacement
* Angular 14 (June 2022)
  * types reactive forms
  * stand alone components,directives,pipes and enhanced template diagnostics
* Angular 15 (Nov 2022)
  * stable standalone API
  * less boiler plate code
* Angular 16 (May 2023)
  * signals
  * jest support
  * mapToCanActivate helper function
* Angular 17 (November 2023)
  * new loop syntax
  * if then else
  * switch
  * block directives
  * deffered rendering
  * SSR and SSG


## Why TS used in Angular

* Type Safety: TypeScript provides static typing, allowing developers to define types for variables, parameters, and return values. This helps catch errors during development and provides better code quality and maintainability.
* IDE Support: TypeScript is supported by most modern IDEs and text editors, providing features like code completion, refactoring tools, and type checking. This improves developer productivity and makes it easier to work with large codebases.
* Enhanced Tooling: TypeScript comes with a rich set of tooling, including a compiler (tsc) that compiles TypeScript code to JavaScript, a language service for editor integration, and various utilities for code analysis and transformation.
* ECMAScript Compatibility: TypeScript is a superset of JavaScript, meaning that any valid JavaScript code is also valid TypeScript code. This allows developers to gradually adopt TypeScript in existing projects and leverage modern JavaScript features while still benefiting from TypeScript's additional capabilities.
* Code Readability and Maintainability: TypeScript's type annotations make code more self-documenting and easier to understand, especially for developers who are new to a codebase. Additionally, TypeScript's features like interfaces and generics promote code reuse and maintainability.
* Community Adoption: TypeScript has gained widespread adoption in the JavaScript community, particularly in frameworks like Angular, React, and Node.js. This means that there is a large ecosystem of libraries, tools, and resources available for TypeScript developers.


## Angular Components

* In Angular, components are the basic building blocks of an application's user interface. 
* They are reusable, self-contained pieces of code that define a portion of the UI and its behavior. 
* Each component encapsulates its own HTML template, CSS styles, and logic, making it easier to manage and maintain complex user interfaces.


## Data Binding in Angular

* In Angular, data binding is a powerful feature that establishes a connection between the application's data and the UI elements that display it. It allows you to synchronize the data between the component class (the TypeScript code) and the template (the HTML code).
* There are several types of data binding supported in Angular:
  * Interpolation (One-Way Binding): 
    * Interpolation allows you to embed expressions in double curly braces ({{ }}) within the HTML template. These expressions are evaluated and their results are inserted into the HTML.
    * `<h1>{{ title }}</h1>`
  * Property Binding (One-Way Binding): 
    * Property binding allows you to bind a property of an HTML element to a property of the component class. You use square brackets ([ ]) to indicate property binding
    * `<img [src]="imageUrl">`
  * Event Binding (One-Way Binding): 
    * Event binding allows you to bind an event of an HTML element to a method in the component class. You use parentheses (( )) to indicate event binding. 
    * `<button (click)="onClick()">Click me</button>`
  * Two-Way Binding: 
    * Two-way binding allows you to establish a bidirectional data flow between a form control element and a component class property. It's achieved using the ngModel directive and the [( )] syntax.
    * `<input [(ngModel)]="name">`
* Data binding in Angular helps to keep the UI and the application's data in sync, reducing boilerplate code and making it easier to build dynamic and responsive web applications.


## Angular Directives

* In Angular, directives are a powerful feature that allows you to extend the functionality of HTML elements or create new reusable components
* Directives can be classified into three types:
* Component Directives:
  * Components are the most common type of directive in Angular.
  * They are used to create reusable and modular UI components.
  * Components consist of a TypeScript class that defines the component's behavior and a template that defines its view.
  * Components are declared using the @Component decorator.
  * ```javascript
	import { Component } from '@angular/core';

	@Component({
	selector: 'app-example',
	template: '<h1>Hello, Angular!</h1>'
	})
	export class ExampleComponent {}
	```
* Attribute Directives: 
  * Attribute directives modify the behavior or appearance of an existing HTML element.
  * They are typically used as attributes within HTML tags.
  * Angular provides several built-in attribute directives such as ngIf, ngFor, and ngStyle.
  * You can also create custom attribute directives to add custom behavior to HTML elements.
  * ```javascript
	import { Directive, ElementRef, HostListener } from '@angular/core';
	@Directive({
	selector: '[appCustomDirective]'
	})
	export class CustomDirective {
	constructor(private el: ElementRef) {}

	@HostListener('mouseenter') onMouseEnter() {
		this.highlight('yellow');
	}

	@HostListener('mouseleave') onMouseLeave() {
		this.highlight(null);
	}

	private highlight(color: string) {
		this.el.nativeElement.style.backgroundColor = color;
	}
	}
  	```
* Structural Directives:
  * Structural directives modify the structure of the HTML by adding, removing, or manipulating elements in the DOM.
  * They are preceded by an asterisk * in the HTML syntax.
  * Angular provides several built-in structural directives such as ngIf and ngFor. 
  * ```javascript
  	<div *ngIf="isVisible">
  		Content is visible
	</div>
	```
## Angular Modules

* Modules play a crucial role in organizing and structuring an application. 
* They help in keeping the codebase manageable, modular, and maintainable
* Types
   *  NgModule (Angular Module)
      *  An NgModule is a class marked by the @NgModule decorator.
      *  It's a container for a cohesive block of code dedicated to a particular application domain, workflow, or closely related set of capabilities.
      *  NgModule can contain components, services, directives, pipes, and other Angular features.
   *  Core Module
      *  Core Module is an NgModule that contains singleton services, components that are used globally throughout the application.
      *  It helps in keeping the AppModule clean and focused on bootstrapping the application.
   *  Shared Module
      * A Shared Module is an NgModule that contains components, directives, and pipes that are shared across multiple modules in the application.
      * It helps in avoiding code duplication and ensures consistency.
* NgModule Metadata
  * declarations: 
    * Contains the list of components, directives, and pipes that belong to this module.
  * imports: 
    * Contains the list of other modules that this module needs to function properly. 
  * exports: 
    * Contains the list of declarations (components, directives, and pipes) that should be accessible to other modules that import this module.
  * providers: 
    * Contains the list of services available to the components of this module.
  * bootstrap: 
    * Defines the root component that Angular should bootstrap when this module is loaded.
  * entryComponents: 
    * Defines components that are not referenced in the HTML but are dynamically created (e.g., via ComponentFactoryResolver).
  * schemas: 
    * Defines the schemas that allow or deny elements and properties to be used in the module.


## Angular CLI

*  command-line tool provided by the Angular team to streamline the development process of Angular applications
*  It simplifies common tasks in Angular development such as project scaffolding, code generation, testing, bundling, and deployment.
*  Project Scaffolding:
   *  `ng new my-app`
*  Code Generation:
   *  `ng generate component my-component`
*  Development Server:
   *  `ng serve`
*  Code Building:
   *  `ng build`
*  Testing:
   *  `ng testing`
*  Linting:
   *  `ng lint`
*  Configuration:
   *  Angular CLI provides configuration files (such as angular.json or tsconfig.json) to customize various aspects of the project, such as build settings, file paths, and more.
*  Dependency Management:
   *  ngular CLI handles dependency management, including installing, updating, and removing dependencies from the project using npm or yarn.
*  Deployment:
   *  Angular CLI facilitates the deployment process by providing optimized build artifacts that can be easily deployed to various hosting platforms.
*  Benifts of using CLI
   *  Productivity
   *  Consistency
   *  Performance
   *  Community Support

  
## Angular Services

* Fundamental part of the architecture and are used to organize and share code across the application
* Services are typically classes with a specific purpose, such as fetching data from a server, logging, or performing calculations.
* They help in keeping components lean and focused on the presentation logic while delegating business logic and data manipulation to the services.
* Characteristics of Angular Services:
  * Singletons
    * meaning that there is only one instance of a service created and shared throughout the application.
  * Dependency Injection (DI)
    * used to provide services to components
    * Services can be injected into components, other services, or even other services.
  * Reusability
    * they encapsulate common functionality that can be used across multiple components.
    * keeping the application DRY (Don't Repeat Yourself).
  * Separation of Concerns
    * Separating business logic, data manipulation, and other non-UI related concerns from the components.
    * This separation makes the codebase easier to maintain, test, and understand.
  * Asynchronous Operations
    * Asynchronous operations such as making HTTP requests to fetch data from a server.
    * Provide a centralized location to manage data fetching and manipulation.
* `ng generate service my-service`


## Depdency Injection in Angular

* It's a technique where one object supplies the dependencies of another object
* Used extensively to create and provide instances of services and other dependencies to components and other parts of the application
* Key concepts:
  * Injection Token
    * Used to identify a dependency when it's registered with Angular's DI system.
    * It's typically represented by a TypeScript token or a string
  * Provider
    * Used to register a dependency with Angular's DI system.
    * It maps an Injection Token to a concrete implementation.
  * Injector
    * The Injector is responsible for instantiating dependencies and injecting them into classes that request them.
    * Angular maintains a hierarchical injector system.
  * Injectable
    * The @Injectable() decorator is used to annotate a class to make it eligible for dependency injection.
    * Services in Angular are typically annotated with `@Injectable()`.
* How Dependency Injection Works in Angular:
  * Registration
    * Dependencies are registered with the Angular DI system using providers.
    * Providers can be registered at the module level or at the component level.
  * Injection
    * When a component, directive, or another service requests a dependency, Angular's injector system looks up the provider for that dependency and creates an instance of it if necessary.
    * It resolves the dependencies of the requested dependency recursively.
  * Hierarchical Injection
    * Angular's DI system works hierarchically.
    * Each Angular application has its own root injector, and each component has its own injector.
    * When a dependency is requested, Angular's injector first looks for it in the local injector of the component.
    * If not found, it traverses up the component tree until it reaches the root injector.
  * Lazy Loading and Scope
    * Angular's DI system supports lazy loading, meaning dependencies are only instantiated when they are needed.
    * Dependencies can have different scopes, such as singleton (shared instance across the application), module (shared within a module), or component (unique instance for each component).
* Benefits of Dependency Injection in Angular:
  * Modularity and Reusability: 
    * Dependency Injection promotes modularity by decoupling components and services, making them easier to understand, maintain, and reuse
  * Testability: 
    * DI facilitates unit testing by allowing dependencies to be easily mocked or replaced with stubs during testing.
  * Flexibility: 
    * Angular's DI system allows for easy swapping of implementations, making it simple to introduce changes or alternate implementations without affecting other parts of the application
