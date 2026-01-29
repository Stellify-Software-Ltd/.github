<p align="center"><a href="https://stellisoft.com" target="_blank"><img src="https://raw.githubusercontent.com/Stellify-Software-Ltd/stellify/refs/heads/main/public/stellify_logo.jpeg" width="200" alt="Stellify Logo"></a></p>

## What is Stellify?

"What if your entire application wasn’t just files containing code, but a dynamic, adaptable blueprint?" 

A system that can evolve and optimize itself, helping you to build faster? 

That’s the power of Stellify. 

Stellify stores code as dynamic JSON definitions. Each definition represents a granular unit of the application— whether it’s a keyword, variable, HTML element, or system setting. 

And that’s not all. We store these definitions in a database instead of a file meaning we get the benefits of structured data—querying, versioning and dynamic updates. 

So, what does this all mean in practice? 

It means that your entire application exists as a structured blueprint, rather than just a bunch of files. 

And Stellify doesn’t just define interfaces and code.

It defines everything. 
Content. 
Configuration. 
System settings. 
Even intent. 

So, what you end up with... is an entire blueprint for your application. 

Now we understand a little about what Stellify is, let’s talk about AI + Stellify 

 This is where things get really exciting. 

Because given a detailed blueprint, AI can create your entire application. 

And more than that... it can continuously refine and improve the result.

Imagine AI optimizing your technology stack as it detects bottlenecks, inefficiencies, or latency issues. 

It can recommend fixes— and adjust your blueprint accordingly. 

All because, and here’s the key: AI has knowledge of your entire application. 

With Stellify, AI understands: 
It understands your intentions. 
Your expectations. 
The consequences of every change. 

It knows if an action in one area... could impact performance, cost, security, or scalability elsewhere. 

It doesn’t just react to problems. It can anticipate them— and recommend the best course of action. 

That, my friends, is Stellify.  

## How Stellify Works

In Stellify’s model, each JSON definition acts as an atomic entity because it represents a fundamental, indivisible unit of the application—whether it’s a keyword, variable, HTML element, or system setting. Since every component is structured in a one-to-one relationship with what it represents, Stellify provides a fully decomposed, structured view of an application that AI can work with more effectively.

This atomic approach has several advantages:

- Precision in AI Processing: Since each definition is atomic, AI can analyze, modify, or generate components without ambiguity.
- Language-Agnostic Representation: The same atomic JSON definitions can be mapped to different languages or frameworks.
- Self-Healing & Maintenance: Changes can be tracked and modified at the smallest functional unit, making updates more reliable.

## Examples of JSON definitions

Here's an example of how we would store an HTML tag using Stellify:

```
{
    type: "layout",
    tag: "div",
    id: "fbc60d5e-e9a2-4c0e-8d09-9a2d196d94fc",
    parent: "b00d4336-1898-4b10-b5f6-aa210ed97bc3",
    children: [
        "4efa4c77-5602-4372-8cf9-3419ada0cf6cm", 
        "71067e7b-7a61-43d0-97c5-1cb51c3ea262"
    ],
    classes: [
        "sm:mx-auto",
        "sm:w-full",
        "sm:max-w-sm",
        "text-white"
    ]
}
```
Notice how in all of the examples the objects are "flat" any nesting that may be required (HTML uses nested tags for example) is achieved by referencing another object, here's example of how we would store the token "for" in PHP: 

```
{
    type: "T_FOR",
    id: "23951891-1b84-4fa9-9f53-fe99faabf08e"
}
```

We don't treat code as nested based on the fact that code statements can be viewed as being nested in text editors. We take the same view of a statement as a compiler would, i.e. we store tokens against a line of code, sequentially. Those lines are in turn referenced by a method or a file. Here's how we would store a PHP file:

```
{
    name: "SocialiteController",
    id: "d441b1e9-28b5-4144-8566-8b924394285a",
    type: "php84",
    extends: "71067e7b-7a61-43d0-97c5-1cb51c3ea262",
    methods: [
        "3e3ae425-4471-400e-ad36-dfeff487a85b"
    ],
    includes: [
        "6177293f-4c34-45d7-8e82-43291fd7c348"
    ]
}
```

Finally, here's an example of how we would store a variable using Javascript as the input language:

```
{
    type: "variable",
    name: "counter",
    id: "0b270c57-3d26-4d89-be5a-91ee11cc5a79"
}
```

## What is stellisoft.com?

[stellisoft.com](https://stellisoft.com/) is the platform, namely the IDE, with which you author your applications using Stellify. It consists of:

- An Interface Builder
- A Code Editor
- A Configuration Editor
- A Bulk Application Editor

Using the Config Editor, you can connect to your own database in order to store your application data (definitions) giving you complete autonomy over your data and how it is used.

## Contributing

Thank you for considering contributing to Stellify! The contribution guide can be found in the [Stellify documentation](https://stellisoft.com/stellify/documentation/contributions).

## Security Vulnerabilities

If you discover a security vulnerability within stellify, please send an e-mail to Matthew Anderson via [matthew.anderson@stellisoft.com](mailto:matthew.anderson@stellisoft.com). All security vulnerabilities will be promptly addressed.

## License

The stellify framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

## Learn more

If you would like to learn more about Stellify then you can read the comprehensive documentation on our website:

- [Configuring routes](https://stellisoft.com/documentation/routes).
- [Building interfaces with HTML and CSS](https://stellisoft.com/documentation/interface-builder).
- [Writing code](https://stellisoft.com/documentation/code-editor).
- [Configuring your application](https://stellisoft.com/documentation/configuration-editor).
- [Performing bulk operations](https://stellisoft.com/documentation/bulk-application-editor).
- [Working with built-in version control](https://stellisoft.com/documentation/version-control).
- [Supports popular web APIs](https://stellisoft.com/documentation/web-apis).
- [Access pre-baked functionality](https://stellisoft.com/documentation/stellify-services).
