# Installation Tailwind CSS
Tailwindcss Install &amp; Configuration Guide. Follow the description below.

![Thumbnail](https://lh3.googleusercontent.com/drive-viewer/AJc5JmS3S2bhn5u41T82MdIaofTtqAUpCa5Hg_Q-YLxiUmxO1pKz7dBfDUO4BPS-Mi-p91I52DJ-HpDgpduxYjKAOVMRtMt3AA=w1366-h649)

## Following in the 7 Step:

#### [`1. Install Tailwind CSS`](#install-tailwindcss)
#### [`2. Configure your template paths`](#configure-paths)
#### [`3. Add the Tailwind directives to your CSS`](#add-css)
#### [`4. Start the Tailwind CLI build process`](#cli-build)
#### [`5. Start using Tailwind in your HTML`](#html-linked)
#### [`6. Run Projects`](#run-project)
#### [`7. VSCODE Tailwindcss Extension`](#vscode-extension)

</br>

#### <a name="install-tailwindcss">**1.** Install Tailwind CSS</a>
First create a folder and open terminal from inside it. And copy and paste the below code in the terminal. ↓↓↓
```bash
npm init -y
npm install -D tailwindcss
npx tailwindcss init
```
</br>

#### <a name="configure-paths">**2.** Configure your template paths</a>
Then go to `tailwind.config.js` in your project and copy and paste the codes below ↓↓↓

```bash
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```
</br>

#### <a name="add-css">**3.** Add the Tailwind directives to your CSS</a>
Then create a folder named `src` in your project and inside it create a file named `input.css` ↓↓↓
```bash
@tailwind base;
@tailwind components;
@tailwind utilities;
```
</br>

#### <a name="cli-build">**4.** Start the Tailwind CLI build process</a>
Then go to the file called `package.json` in your project and then copy and paste the below code inside the section called `scripts` ↓↓↓

```bash
"tailwindcss": "tailwindcss -i ./src/input.css -o ./dist/output.css -w"
```
</br>

#### <a name="html-linked">**5.** Start using Tailwind in your HTML</a>
Then create a file called `index.html` in your project and copy and paste the below code inside it. ↓↓↓

```bash
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Tailwind Projects</title>
    <link rel="icon" href="../image/tailwindcss-logo.svg" type="image/x-icon" />
    <link rel="stylesheet" href="../dist/output.css" />
  </head>
  <body class="h-screen flex items-center justify-items-center bg-blue-200">
    <div class="m-auto max-w-xl px-28 py-16 rounded-xl bg-gradient-to-r from-white to-blue-200">
      <p class="text-3xl"><b>Hello!</b> Tailwind CSS</p>
    </div>
  </body>
</html>
```
</br>

#### <a name="run-project">**6.** Run Projects</a>
Finally, type `npm run tailwindcss` from your project's terminal and then open the `index.html` file in the browser. ↓↓↓

```bash
npm run tailwindcss
```
</br>

#### <a name="vscode-extension">**7.** VSCODE Tailwindcss Extension</a>
Search `Tailwind CSS IntelliSense` in the editor to install the Tailwind CSS extension within `Visual Studio Code`

```bash
Tailwind CSS IntelliSense
```

![Tailwind CSS IntelliSense](https://lh3.googleusercontent.com/drive-viewer/AJc5JmRueA-kP6ukVIziTZEwqAtKWmMsUGdBCKcyn0JnLKmiEOtJzRT98uII2aPeQfJUyFkLNaMmXrsLBWQbiBNEiERLbfHSHQ=w1366-h649)

- #### _Extra configuration for Tailwind CSS language to avoid error or warning in VScode._
  Copy the code below and paste it into the `settings.json` file from the `.vscode` folder in your project. ↓↓↓

```bash
// Tailwindcss related config
"css.validate": false,
"tailwindCSS.emmetCompletions": true
```
</br>

𝔸𝕝𝕝 𝕕𝕠𝕟𝕖! 𝕋𝕙𝕒𝕟𝕜𝕤 𝕪𝕠𝕦..
