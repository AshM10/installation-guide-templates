# TailwindCSS in React

## Installation

To install tailwindcss on a react app using yarn, follow these steps:

1. Open a terminal window and navigate to the root directory of your react app.
2. Run the following command to install tailwindcss as a development dependency:

``` yarn add tailwindcss -D ```

3. Next, create a configuration file for tailwindcss by running the following command:

``` npx tailwindcss init ```

This will create a tailwind.config.js file in the root directory of your project.

4. Next, create a new file called tailwind.css in your project's src directory and add the following lines of code:

```js
@import "tailwindcss/base";
@import "tailwindcss/components";
@import "tailwindcss/utilities";
```

5. In your index.js file, import the tailwind.css file as follows:

``` import "./tailwind.css"; ```

6. Finally, run the following command to build your tailwindcss styles:

``` npx tailwindcss build src/tailwind.css -o src/tailwind.output.css ```

This will generate an output file called tailwind.output.css that contains the compiled tailwindcss styles. You can then reference this file in your HTML file or import it into your react components as needed.

## Resources

- [Tailwind CSS Official Docs](https://tailwindcss.com)
