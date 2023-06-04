# Process

# setup tailwind

create folder structure

tailwind.config.js

- Create a project folder.
- Navigate to the project folder in the terminal.
- Initialize a new npm project by running: npm init -y.
- Install Tailwind CSS and its dependencies by running: npm install tailwindcss postcss autoprefixer.
- Generate a Tailwind CSS configuration file by running: npx tailwindcss init.
- Create a CSS file (e.g., styles.css) in your project folder.
- Add the following code to styles.css:
`@import 'tailwindcss/base';
@import 'tailwindcss/components';
@import 'tailwindcss/utilities';`

- Create an HTML file (e.g., index.html) in your project folder.
- Link the styles.css file and any other necessary files (e.g., JavaScript) in index.html.
- Build the CSS file by running: npx tailwindcss build styles.css -o output.css.
- Include the compiled output.css file in your HTML file.
- Start a development server to preview your project.
- edit package.json to include
`"scripts": {
    "tailwind": "npx tailwindcss -i ./src/input.css -o ./build/css/style.css --watch",
    "prettier": "npx prettier --write **/*.html"
  },`
- edit tailwind.config.js to include
`content: ["./build/*.html"],`

# styles used
margins
padding
borders
linear gradients
radial gradient (using css)
flexbox
position in row, then column reverse order
grid
radius / circular items
images
sizeing elements in fractions of their original size
dark mode / light mode
center text
colouring built in colours and weight
bold font
shadow - drop shadow
rounded
hidden display
block display

