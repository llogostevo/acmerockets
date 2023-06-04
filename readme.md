# Process

# Setup Tailwind (2023 - May)

If setting up a totally new project the following steps can be carried out

create folder structure
 - root project folder
 - - build
 - - - css
 - - - img
 - - src
 - tailwind.config.js
 - readme.md

- Create a project folder.
- Navigate to the project folder in the terminal.
- Initialize a new npm project by running: `npm init -y`
- Install Tailwind CSS and its dependencies by running: 
`npm install -D tailwindcss@latest postcss@latest autoprefixer@latest`
- Generate a Tailwind CSS configuration file by running:
 `npx tailwindcss init`.
 - edit tailwind.config.js to include, (create file inside root project if not there)
`content: ["./build/*.html"],`
- Create a CSS folder inside a folder called `build` file (e.g., styles.css) in your project folder.
- Add the following code to styles.css:
`@import 'tailwindcss/base';
@import 'tailwindcss/components';
@import 'tailwindcss/utilities';`

- Create an HTML file (e.g., index.html) in your project folder.
- Link the styles.css file and any other necessary files (e.g., JavaScript) in index.html.
- Build the CSS file by running: `npx tailwindcss build styles.css -o output.css`.
- Include the compiled output.css file in your HTML file.
- Start a development server to preview your project.
- edit package.json to include
`"scripts": {
    "tailwind": "npx tailwindcss -i ./src/input.css -o ./build/css/style.css --watch",
    "prettier": "npx prettier --write **/*.html"
  },`

  - test tailwind works on the server
  - create a `.gitignore` file and include
  `node_modules`
  - setup git and connect to github


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
figure element html

# other techniques
- adding a custom class using @layer utilities
- making a media query from the class in tailind.config.js - using extend and adding a name for hte screen sizes
- calculat



