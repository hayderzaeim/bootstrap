# NABU Tool


## Introduction
NABU is a powerful tool that aims to simplify the process of writing code for creating HTML elements in a manner similar to JSON, while also facilitating the organization and maintainability of web development projects. It supports JavaScript , making it a versatile solution for web developers.

One of the key features of NABU Tool is its ability to represent HTML elements using a JSON-like syntax. This allows developers to define and structure their HTML elements in a more intuitive and readable way, resembling the structure of JSON objects. This approach eliminates the need for writing repetitive HTML markup and instead focuses on creating objects that represent the desired structure of the elements. This not only enhances code readability but also promotes better organization and maintainability of the codebase.

By encapsulating the creation and manipulation of HTML elements within the NABU Tool, it provides a modular and reusable approach to web development. Developers can leverage the Tool's functions and methods to dynamically generate HTML elements, set attributes, define child elements, and apply styles. This modular approach promotes code reusability and helps developers write cleaner, more structured code.

Furthermore, NABU Tool promotes extensibility and scalability. With its modular architecture, developers can easily extend the Tool's functionality by adding custom methods or modifying existing ones to suit their specific needs. This flexibility allows for the growth and adaptation of the Tool as projects evolve over time. Developers can build upon the foundation provided by NABU and create robust, scalable web applications.


NABU tool is a self-contained solution that does not rely on external dependencies or external links. Its primary purpose is to generate HTML code using the JSON method, enabling a more organized and scalable file structure for projects. It seamlessly integrates with Bootstrap and provides an enhanced feature set, particularly for simplified front-end development. This advantage makes Bootstrap a preferred choice over other frameworks


## Installation
To use the NABU Tool, you need to include the nabu.js file in your project. You can download the file and place it in your project directory. Then, you can import the Tool in your JavaScript code using the following syntax:

## Usage
Here is an example of how to use NABU Tool:

```javascript
   import { NABU } from './nabu.js';
```

## Usage
Once you have imported the NABU Tool, you can start using its functions and methods to create and manipulate HTML elements. Here are some examples:

## Creating elements in the head
You can use the NABU.head() method to create elements in the <head> section of your HTML document. It accepts an object representing the elements to be created. Each key in the object represents the HTML tag name, and the corresponding value represents the attributes and child elements of that tag. For example:

```javascript
NABU.head({
    title: {
        text: 'Document'
    },
    meta: {
        charset: 'UTF-8'
    }
});
```


## Creating elements in the body
Similarly, you can use the NABU.body() method to create elements in the <body> section of your HTML document. It follows the same syntax as NABU.head(). Additionally, you can provide attributes for the parent element as the second argument. For example:

```javascript
NABU.body(
    {
        div: {
            id: 'loginPage',
            class: 'loginPage',
            child: [
                {
                    form: {
                        id: 'loginForm',
                        class: 'loginForm',
                        child: [
                            {
                                h2: {
                                    id: 'h2hayder',
                                    text: 'hayder zaeem',
                                },
                            },
                            // Other child elements...
                        ],
                    },
                },
            ],
        },
    },
    {
        id: 'hayder',
        style: {
            margin: '0px',
            background: '#ccc'
        }
    }
);
```

## Importing data from a file
The NABU.getFiler() method allows you to import data from a file. It accepts the file path and the name of the function to be executed. For example:

```javascript
NABU.getFiler('../path', 'name function');

```

## Creating child elements
You can use the NABU.child() method to create child elements. It accepts an array of objects, where each object represents a child element to be created. For example:

```javascript
NABU.child([
    {
        h2: {
            id: 'id1',
            text: 'hayder zaeem',
        }
    },
    // Other child elements...
]);

```
## Creating a single element
You can use the NABU.element() method to create a single element. It follows the same syntax as NABU.body() but creates only one element. For example:

```javascript
NABU.element({
    div: {
        id: 'loginPage',
        class: 'loginPage',
        child: [
            {
                h2: {
                    id: 'id1',
                    text: 'hayder zaeem',
                }
            }
        ]
    }
});

```
These are some of the basic functionalities provided by the NABU Tool. You can explore more features and options by referring to the Tool's documentation or source code.




