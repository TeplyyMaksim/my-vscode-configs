# my-vscode-configs
All VSCode configs for comfort work

## Theme:
``One Dark Pro``

## Packages:
* Angular Essentials
* TypeScript Hero
* Path Autocomplete
* Git Lens
* TODO Highlight

## Workspace settings:
    {
      "explorer.openEditors.visible": 0

      /* Indent settings */
      "editor.insertSpaces": true,
      "editor.tabSize": 2,
      "editor.detectIndentation": true,

      "todohighlight.keywords": [
        {
          "text": "NOTE:",
          "color": "#3174ad",
          "backgroundColor": "#00fa9a"
        }
      ]
    }

## Snippets:
### React:
    {
        /*
            // Place your snippets for JavaScript React here. Each snippet is defined under a snippet name and has a prefix, body and 
            // description. The prefix is what is used to trigger the snippet and the body will be expanded and inserted. Possible variables are:
            // $1, $2 for tab stops, $0 for the final cursor position, and ${1:label}, ${2:another} for placeholders. Placeholders with the 
            // same ids are connected.
        */
        "ES6 Component": {
            "prefix": "rc",
            "body": [
                "import React, { Component } from 'react';",
                "",
                "export default class NewComponent extends Component {",
                "",
                "\tstate = { someKey: 'Some Value' };",
                "",
                "\trender() {",
                "\t\treturn <div></div>;",
                "\t}",
                "}"
            ],
            "description": "ES6 Component"
        },

        "ES6 Function Component": {
            "prefix": "rfc",
            "body": [
                "import React from 'react';",
                "",
                "export default ({ property }) =>",
                "\t<div>{property}</div>;",
            ],
            "description": "ES6 Function Component"
        },

        "ES6 Constructor Component": {
          "prefix": "rcc",
            "body": [
              "import React, { Component } from 'react';",
              "",
              "export default class NewComponent extends Component {",
              "\tconstructor(props) {",
              "\t\tsuper(props);",
              "",
              "\t\tthis.state = {",
              "\t\t\tsomeKey: 'Some Value'",
              "\t\t};",
              "",
              "\t\t// this.someMethod = this.someMethod.bind(this);",
              "\t}",
              "",
              "\trender() {",
              "\t\treturn <div></div>;",
              "\t}",
              "}"
            ],
            "description": "ES6 Constructor Component"
        },
    }
### HTML:
    {
    /*
      // Place your snippets for HTML here. Each snippet is defined under a snippet name and has a prefix, body and 
      // description. The prefix is what is used to trigger the snippet and the body will be expanded and inserted. Possible variables are:
      // $1, $2 for tab stops, $0 for the final cursor position, and ${1:label}, ${2:another} for placeholders. Placeholders with the 
      // same ids are connected.
    */
      "Link without redirect": {
        "prefix": "lwr",
        "body": [
          "<a href=\"javascript:void(0)\">$1</a>$0"
        ],
        "description": "Link without redirect"
      }
    }
