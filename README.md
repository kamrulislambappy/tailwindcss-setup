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
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tailwindcss Projects</title>
    <link rel="stylesheet" href="./dist/output.css">
</head>
<body class="">
    <div
        class="m-60 p-10 text-xl font-semibold text-center border-2 rounded-xl bg-gray-900 text-cyan-200 border-sky-400">HELLO! Tailwind CSS</div>
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

![Tailwind CSS IntelliSense](https://lh3.googleusercontent.com/drive-viewer/AJc5JmRueA-kP6ukVIziTZEwqAtKWmMsUGdBCKcyn0JnLKmiEOtJzRT98uII2aPeQfJUyFkLNaMmXrsLBWQbiBNEiERLbfHSHQ=w1366-h649)

```bash
Tailwind CSS IntelliSense
```
</br>

𝔸𝕝𝕝 𝕕𝕠𝕟𝕖! 𝕋𝕙𝕒𝕟𝕜𝕤 𝕪𝕠𝕦..
