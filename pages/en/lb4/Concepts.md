---
lang: en
title: 'Key concepts'
keywords: LoopBack 4.0, LoopBack 4
tags:
sidebar: lb4_sidebar
permalink: /doc/en/lb4/Concepts.html
summary:
---

LoopBack 4 introduces some new concepts that are important to understand:

* [**Application**](Application.html): In LoopBack 4, the Application class is
  the central class for setting up all of your module’s components, controllers,
  servers and bindings. The Application class extends [Context](Context.html), and
  provides the controls for starting and stopping itself and its associated
  servers.
* [**Server**](Server.html): Represents implementation for inbound transports and/or protocols such as REST over http, gRPC over http2, and graphQL over https. It typically listens for requests on a specific port, handle them, and return appropriate responses.
* [**Context**](Context.html): An abstraction of all state and dependencies in your application, that LoopBack uses to “manage” everything. It's a global registry for everything in your app (configurations, state, dependencies, classes, and so on).
* [**Dependency Injection**](Dependency-injection.html): Technique that separates the construction of dependencies of a class or function from its behavior, to keep the code loosely coupled.
* [**Booting an Application**](Booting-an-Application.html): A convention-based
  bootstrapper that can find and bind artifacts such as Controllers, Repositories, etc.
* [**Controller**](Controllers.html): Class that implements operations defined by application’s REST API. It implements an application’s business logic and acts as a bridge between the HTTP/REST API and domain/database models. A Controller operates only on processed input and abstractions of backend services / databases.
* [**Route**](Routes.html): Mapping between your API specification and an Operation (JavaScript implementation). It tells LoopBack which function to invoke() given an HTTP request.
* [**Sequence**](Sequence.html): A stateless grouping of [Actions](Sequence.html#actions) that control how a Server responds to requests.
* [**Model**](Model.html): Represents the definition of a model in LoopBack, with respect to the datasource juggler. The `@loopback/repository` module provides special decorators for adding metadata to TypeScript/JavaScript classes to use them with the legacy implementation of Datasource Juggler. In addition, `@loopback/repository-json-schema` module uses the decorators' metadata to build a matching JSON Schema.
* [**Repository**](Repositories.html): Type of Service that represents a collection of data within a DataSource.
* [**Decorator**](Decorators.html): Enables you to annotate or modify your class declarations and members with metadata.
* **Component**: A package that bundles one or more Loopback extensions.
  * See [Using components](Using-components.html) and [Creating components](Creating-components.html) for more information.

{% include note.html title="Review Note" content="_Perhaps this should include some of the material in <a href='Thinking-in-LoopBack.html'> Thinking in LoopBack</a>_.
" %}
