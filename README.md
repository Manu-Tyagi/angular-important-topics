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
  - [Angular Template](#angular-template)
  - [Angular Router](#angular-router)
  - [Angular Pipes](#angular-pipes)
  - [Angular Forms](#angular-forms)
  - [Angular Life Cycle](#angular-life-cycle)
  - [Eager Loading vs Lazy Loading](#eager-loading-vs-lazy-loading)
  - [Angular Guards](#angular-guards)
  - [Angular Interceptor](#angular-interceptor)
  - [Zone js in Angular](#zone-js-in-angular)
  - [Angular Universal](#angular-universal)
  - [Angular Change Detection Strategies](#angular-change-detection-strategies)


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


## Angular Template

* Templates in Angular are HTML files with additional syntax and features provided by Angular for data binding, directives, and other functionalities
* Features of Angular Templates
  * Data Binding
    * Angular templates support various types of data binding, including interpolation ({{}}), property binding ([property]="value"), event binding ((event)="handler()"), and two-way binding ([(ngModel)]).
  * Directives
    * Angular templates can include Angular directives, which are instructions in the DOM that tell Angular how to modify the behavior or appearance of HTML elements.
    * Directives like ngIf, ngFor, and ngClass are commonly used in Angular templates.
  * Template Expressions
    * Templates can contain expressions that are evaluated against the component's context. 
    * These expressions can perform simple calculations, access properties and methods of the component class, and interact with template variables.
  * Template Statements
    * Alongside expressions, templates support statements for event handling and flow control. 
    * For example, you can use *ngIf, *ngFor, and *ngSwitch to conditionally render elements.
  * Template Reference Variables
    * Angular templates allow you to create reference variables using the # symbol, which can be used to access elements or directives within the template.
  * Template Interpolation
    * Interpolation is a way to output data from the component class into the HTML template. 
    * It's achieved by wrapping the expression in double curly braces ({{ expression }})


## Angular Router

* Module provided by Angular for managing navigation and routing in Angular applications 
* Allows developers to define navigation paths, map them to specific components, and handle navigation events seamlessly
* Importance
  * Client-Side Routing
    * Angular Router enables client-side routing, allowing users to navigate between different views of an application without full page reloads. 
    * This results in faster navigation and better user experience.
  * Single Page Application (SPA) Support
    * Angular Router is essential for building Single Page Applications (SPAs) where the entire application is loaded once, and subsequent navigation occurs within the same page. 
    * This approach improves performance and reduces server load.
  * Nested Routing and Lazy Loading
    * Angular Router supports nested routing, allowing developers to define routes hierarchically. Nested routes help in organizing complex applications with multiple levels of navigation.
    * It also supports lazy loading of modules, allowing you to load parts of your application asynchronously when needed, improving initial load time and reducing the size of the main bundle.
  * Route Parameters and Data Resolvers
    * Angular Router allows passing parameters in routes, enabling dynamic routing based on user input or application state.
    * It supports data resolvers, allowing developers to fetch necessary data before navigating to a route, ensuring that the route components have the required data when they render.
  * Route Guards
    * Angular Router provides route guards, which are used to protect routes based on certain conditions. 
    * Route guards can prevent unauthorized access, perform authentication, and execute additional logic before activating a route
  * HTML5 History API Integration
    * Angular Router integrates with the HTML5 History API, enabling support for features like browser history manipulation, bookmarking, and deep linking
  * Navigation Events and Lifecycle Hooks
    * Angular Router emits events for various navigation actions, such as route activation, deactivation, and navigation start/end
    * Developers can subscribe to these events and perform additional actions as needed.
    * Route lifecycle hooks, such as OnInit, OnDestroy, and OnActivate, allow developers to execute code at specific points in the lifecycle of a route component.
  * SEO (Search Engine Optimization)
    * Angular Router supports server-side rendering and pre-rendering techniques, which are crucial for improving SEO and ensuring that search engine crawlers can index the content of Angular applications effectively

## Angular Pipes

* Angular Pipes are a feature provided by Angular that allows developers to transform and format data within a template. 
* Pipes are used in template expressions to modify the output of data before displaying it to the user. 
* Angular comes with several built-in pipes, and developers can also create custom pipes to suit specific application needs.
* Key Features of Angular Pipes
  * Transformation of Data
    * Pipes are used to transform the data before displaying it in the template. 
    * They can be used to format strings, numbers, dates, and other types of data.
  * Chaining
    * Multiple pipes can be chained together to perform multiple transformations on the data in a single expression.
  * Parameterization
    * Pipes can accept parameters to customize their behavior. Parameters are passed to the pipe using colon (`:`) syntax
  * Pure and Impure Pipes
    * Angular pipes can be either pure or impure.
    * Pure pipes are stateless and only recalculate the output when the input data changes. They are more efficient and are the default type of pipe.
    * Impure pipes can have internal state and can execute more frequently, even on every change detection cycle.
  * Built-in pipes example
    * DatePipe
    * UpperCasePipe and LowerCasePipe
    * CurrencyPipe
    * DecimalPipe and PercentPipe
    * AsyncPipe
    * SlicePipe
  * Custom Pipes Example
```javascript
// capitalize.pipe.ts
import { Pipe, PipeTransform } from '@angular/core';

@Pipe({
  name: 'capitalize'
})
export class CapitalizePipe implements PipeTransform {
  transform(value: string): string {
    if (!value) return ''; // return empty string if value is null, undefined, or empty

    return value.replace(/\b\w/g, firstLetter => firstLetter.toUpperCase());
  }
}
```

## Angular Forms

* There are two types of forms in angular
  * Template Driven Forms
    * Template-driven forms rely on directives in the template to create and manipulate the form's structure and data model
    * These forms are easier to get started with and are suitable for simpler forms with less complex validation requirements
    * Template-driven forms use Angular directives like ngModel, ngForm, and ngSubmit to bind form controls to the data model and handle form submission
    * The form controls are automatically synchronized with the data model, making it easy to access and manipulate form data in the component class
    * Template-driven forms require less boilerplate code compared to reactive forms, making them quicker to set up and easier to maintain for simple form
  * Reactive Form
    * Reactive forms are based on a reactive programming model, where the form controls are created and managed programmatically in the component class. 
    * These forms offer more flexibility and control over form validation and complex form scenarios.
    * Reactive forms use instances of the FormControl, FormGroup, and FormArray classes to represent form controls, groups, and arrays programmatically.
    * Validation logic is defined explicitly in the component class using validators provided by Angular or custom validator functions.
    * Reactive forms promote immutability, which makes it easier to track changes to form data and perform operations like undo/redo.
    * Reactive forms are more suitable for dynamic forms where form controls may be added or removed based on user interaction or data changes.


## Angular Life Cycle

* ngOnChanges(): This method is called when Angular sets or resets data-bound input properties. It receives a SimpleChanges object containing the previous and current values of the input properties.

* ngOnInit(): This method is called after Angular has initialized all data-bound properties of the component. It is a good place to perform initialization logic for the component.

* ngDoCheck(): This method is called during every change detection run, which can be triggered by various events in the application. It allows you to implement custom change detection logic.

* ngAfterContentInit(): This method is called after Angular has projected external content into the component's view (e.g., content projection using `<ng-content>`).

* ngAfterContentChecked(): This method is called after Angular has checked the projected content of the component.

* ngAfterViewInit(): This method is called after Angular has fully initialized the component's view and its child views. It is a good place to perform initialization logic that relies on the view being initialized.

* ngAfterViewChecked(): This method is called after Angular has checked the component's view and its child views.

* ngOnDestroy(): This method is called just before Angular destroys the component. It is a good place to clean up resources such as event listeners or subscriptions to avoid memory leaks.


## Eager Loading vs Lazy Loading

* Eager Loading
  * By default, Angular modules are eagerly loaded, meaning that they are loaded as soon as the application starts.
  * Eager loading is suitable for modules that are essential for the application to function properly, such as the root module (AppModule).
* Lazy Loading
  * Lazy loading allows Angular to load modules asynchronously when the user navigates to a specific route that requires those modules.
  * Lazy loading can significantly improve the initial loading time of the application by only loading the necessary modules when they are needed.
  * To lazy load a module, you configure the route to load that module using the loadChildren property of the route configuration.
* Preloading Strategies:
  * Angular provides options to preload lazy-loaded modules in the background after the initial load of the application, which can improve the user experience by reducing the loading time when navigating between different sections of the application.
  * There are different preloading strategies such as PreloadAllModules, NoPreloading, and custom preloading strategies.


## Angular Guards

* CanActivate
  * `CanActivate` guard determines whether a route can be activated or not. It's used to protect routes from being accessed by unauthorized users.
  * Used for implementing authentication and authorization logic to allow or deny access to certain routes based on the user's credentials or permissions.
  * The guard can return a boolean value, a `Promise<boolean>`, or an `Observable<boolean>`.
* CanActivateChild
  * CanActivateChild guard is similar to CanActivate, but it's specifically designed for protecting child routes of a parent route.
  * Used when you want to apply the same authorization logic to all child routes of a parent route.
* CanDeactivate
  * CanDeactivate guard determines whether a route can be deactivated or not. It's used to prevent users from leaving a route with unsaved changes.
  * It's commonly used in forms or wizards where you want to prompt users with a confirmation dialog before they navigate away from the page.
* CanLoad
  * CanLoad guard is used to prevent lazy-loaded modules from being loaded until certain conditions are met.
  * It's useful for implementing access control to lazy-loaded modules, where you want to check whether a user is authorized to load the module before it's fetched from the server.
* Resolve
  * Resolve guard is used to fetch asynchronous data before the route is activated.
  * It's often used to prefetch data required by a component so that the component can be fully initialized with data before being displayed to the user.
  * The guard resolves the data before the route is activated, ensuring that the resolved data is available to the component.


## Angular Interceptor

* Angular Interceptors provide a way to intercept HTTP requests or responses globally or per-request basis.
* They are powerful tools for adding behavior to HTTP requests and responses, such as modifying headers, handling errors, logging, caching, and more
* HTTP Interceptors
  * HTTP Interceptors are Angular services that implement the HttpInterceptor in
  * 
  * terface.
  * They intercept HTTP requests or responses processed by the Angular HttpClient.
  * Interceptors can be used to modify outgoing requests, intercept responses, and handle errors.
  * You can create custom interceptors to add common functionality across multiple HTTP requests.
* Common use case
  * Authentication: Interceptors can add authentication tokens to outgoing requests or handle unauthorized responses.
  * Logging: Interceptors can log request and response data for debugging purposes.
  * Error Handling: Interceptors can intercept error responses and handle them in a consistent way, such as displaying error messages to the user.
  * Caching: Interceptors can cache responses to avoid redundant requests to the server.
  * Request Transformation: Interceptors can transform outgoing requests, such as adding headers or modifying the request body.
* You can chain multiple interceptors together to apply different behaviors to HTTP requests and responses.
* To create an interceptor, you need to implement the HttpInterceptor interface, which requires you to implement the intercept method.
* Interceptors need to be registered with the Angular dependency injection system.
You can register interceptors globally in the AppModule by providing them in the HTTP_INTERCEPTORS multi-provider token.


## Zone js in Angular

* `zone.js` is a critical part of Angular's architecture, providing the infrastructure needed for reactive change detection, error handling, and seamless integration with asynchronous operations. 
* It abstracts away the complexities of managing asynchronous tasks and ensures that Angular applications remain responsive and performant.


## Angular Universal

* Angular Universal is a technology provided by the Angular framework that allows developers to render Angular applications on the server-side. 
* Traditionally, Angular applications run entirely in the browser, but Angular Universal extends Angular's capabilities to support server-side rendering (SSR).
* SSR can improve the perceived performance of Angular applications by reducing the time it takes for the initial content to be displayed to the user.
* SSR ensures that the application's content is available to search engine crawlers and social media bots, which might not execute JavaScript.


## Angular Change Detection Strategies

* Angular, change detection is the mechanism by which Angular detects changes in the application state and updates the DOM to reflect those changes.
* Default (Automatic) Change Detection 
  * Angular's default change detection strategy, also known as automatic change detection, triggers change detection for all components in the application tree whenever an event, HTTP request, or other asynchronous operation occurs.
  * Angular automatically checks all components and their child components for changes on every browser event, such as mouse movements, keyboard inputs, timers, and XHR responses.
* OnPush Change Detection
  * When using the OnPush strategy, Angular only checks a component for changes if one of its input properties has changed or if an event originated from the component or one of its children.
  * Components using OnPush change detection must explicitly notify Angular of changes by using immutable data structures or triggering change detection manually using ChangeDetectorRef.
  * This strategy can significantly improve the performance of applications by reducing the number of change detection checks and unnecessary DOM updates.
* Noop Change Detection
  * The Noop (No Operation) change detection strategy disables change detection entirely for a component and its subtree.
  * When using the Noop strategy, Angular does not check for changes in the component's properties or trigger any change detection mechanisms
  * This strategy is useful for scenarios where you want to manage change detection manually or optimize performance by bypassing Angular's change detection entirely.
* Detached Change Detection
  * The Detached change detection strategy is similar to Noop, but it allows you to manually trigger change detection for a component and its subtree.
  * Components using the Detached strategy are not checked for changes automatically by Angular, but you can trigger change detection manually using ChangeDetectorRef.
  * This strategy provides more control over change detection and can be useful for optimizing performance in specific scenarios.
* 