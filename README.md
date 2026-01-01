<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/siamahnaf/assets-kit/main/logo/logo-white.png">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/siamahnaf/assets-kit/main/logo/logo-black.png">
  <img alt="Siam Ahnaf" src="https://raw.githubusercontent.com/siamahnaf/assets-kit/main/logo/logo-black.png" height="auto" width="240">
</picture>

# React Tailwindcss Datepicker

<p align="center">
    <a href="https://react-tailwindcss-datepicker.vercel.app/" target="_blank">
      <img alt="React Tailwindcss Datepicker" width="100" style="border-radius: 100%;" src="https://raw.githubusercontent.com/onesine/react-tailwindcss-datepicker/master/assets/img/calendar_logo.svg?raw=true">
    </a><br><br>
    A modern date range picker component for React using Tailwind 3 and dayjs. Alternative to Litepie Datepicker which uses Vuejs.
</p>

<div align="center">
    
[![npm version](https://img.shields.io/npm/v/react-tailwindcss-datepicker?style=flat-square)](https://www.npmjs.com/package/react-tailwindcss-datepicker)
[![npm downloads](https://img.shields.io/npm/dt/react-tailwindcss-datepicker?style=flat-square)](https://www.npmjs.com/package/react-tailwindcss-datepicker)
    
</div>

## Contents
* [Features](#features)
* [Documentation](#documentation)
* [Installation](#installation)
* [Simple Usage](#simple-usage)
* [Theming Options](#theming-options)
* [Playground](#playground)
* [Contributing](#contributing)

##  Features
- ✅ Theming options
- ✅ Dark mode
- ✅ Single Date
- ✅ Single date use Range
- ✅ Shortcuts
- ✅ TypeScript support
- ✅ Localization(i18n)
- ✅ Date formatting
- ✅ Disable specific dates
- ✅ Minimum Date and Maximum Date
- ⬜ Custom shortcuts

## Documentation

Go to [full documentation](https://react-tailwindcss-datepicker.vercel.app/)

## Installation

⚠️ React Tailwindcss Datepicker uses Tailwind CSS 3 (with the [@tailwindcss/forms](https://github.com/tailwindlabs/tailwindcss-forms) plugin) & [Dayjs](https://day.js.org/en/) under the hood to work.

### Install via npm

```
$ npm install react-tailwindcss-datepicker 
```

### Install via yarn

```
$ yarn add react-tailwindcss-datepicker 
```

Make sure you have installed the peer dependencies as well with the below versions.
```
"dayjs": "^1.11.6",
"react": "^17.0.2 || ^18.2.0"
```

## Simple Usage

#### Tailwindcss Configuration
Add the datepicker to your tailwind configuration using this code

```javascript
// in your tailwind.config.js
module.exports = {
    // ...
    content: ["./src/**/*.{js,jsx,ts,tsx}", "./node_modules/react-tailwindcss-datepicker/dist/index.esm.js"],
    // ...
}
```

Then use react-tailwindcss-select in your app:

```jsx
import React, {useState} from "react";
import Datepicker from "react-tailwindcss-datepicker";

const App = () => {
    const [value, setValue] = useState({
        startDate: new Date(),
        endDate: new Date().setMonth(11)
    });
    
    const handleValueChange = (newValue) => {
        console.log("newValue:", newValue);
        setValue(newValue);
    }
    
    return (
        <div>
            <Datepicker
                value={value}
                onChange={handleValueChange}
            />
        </div>
    );
};

export default App;
```

## Theming options

**Light Mode**

![Light Mode](https://raw.githubusercontent.com/onesine/react-tailwindcss-datepicker/master/assets/img/Screen_Shot_2022-08-04_at_17.04.09_light.png?raw=true)

**Dark Mode**

![Dark Mode](https://raw.githubusercontent.com/onesine/react-tailwindcss-datepicker/master/assets/img/Screen_Shot_2022-08-04_at_17.04.09_dark.png?raw=true)

**Supported themes**
![Theme supported](https://raw.githubusercontent.com/onesine/react-tailwindcss-datepicker/master/assets/img/Screen_Shot_2022-08-04_at_17.04.09_theme.png?raw=true)

**Teal themes example**
![Theme supported](https://raw.githubusercontent.com/onesine/react-tailwindcss-datepicker/master/assets/img/Screen_Shot_2022-08-04_at_17.04.09_teal.png?raw=true)

You can find the demo at [here](https://react-tailwindcss-datepicker.vercel.app/demo)

> **Info**
>
> 👉 To discover the other possibilities offered by this library, you can consult the [full documentation](https://react-tailwindcss-datepicker.vercel.app/).


## PlayGround

Clone the `master` branch and run commands:

```sh
# Using npm
npm install && npm dev

# Using yarn
yarn install && yarn dev

```

Open a browser and navigate to `http://localhost:8888`

## Contributing

See [CONTRIBUTING.md](https://github.com/onesine/react-tailwindcss-datepicker/blob/master/CONTRIBUTING.md)

## Official Documentation repo
[https://github.com/onesine/react-tailwindcss-datepicker-doc](https://github.com/onesine/react-tailwindcss-datepicker-doc)


## Connect with me
<div style="display: flex; align-items: center; gap: 3px;">
<a href="https://wa.me/8801611994403"><img src="https://raw.githubusercontent.com/siamahnaf/assets-kit/main/icons/whatsapp.png" width="40" height="40"></a>
<a href="https://siamahnaf.com/" style="margin-right: 8px"><img src="https://raw.githubusercontent.com/siamahnaf/assets-kit/main/icons/web.png" width="40" height="40"></a>
<a href="https://www.linkedin.com/in/siamahnaf/" style="margin-right: 8px"><img src="https://raw.githubusercontent.com/siamahnaf/assets-kit/main/icons/linkedin.png" width="40" height="40"></a>
<a href="https://x.com/siamahnaf198" style="margin-right: 8px"><img src="https://raw.githubusercontent.com/siamahnaf/assets-kit/main/icons/x.png" width="40" height="40"></a>
<a href="https://www.facebook.com/siamahnaf198/" style="margin-right: 8px"><img src="https://raw.githubusercontent.com/siamahnaf/assets-kit/main/icons/facebook.png" width="40" height="40"></a>
<a href="https://t.me/siamahnaf198" style="margin-right: 8px"><img src="https://raw.githubusercontent.com/siamahnaf/assets-kit/main/icons/telegram.png" width="40" height="40"></a>
<a href="https://www.npmjs.com/~siamahnaf" style="margin-right: 8px"><img src="https://raw.githubusercontent.com/siamahnaf/assets-kit/main/icons/npm.png" width="40" height="40"></a>
</div>


------------

<p align="center" color="red"><a href="https://www.siamahnaf.com/">www.siamahnaf.com</a></p>