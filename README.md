# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

                 <-------------------------------------------------->
                                   ************





              **How to deploy project from local to github and than to Render.com**

1. create one new Repositorie on Github

2. if you are using visual studio code, than clone it. ( git clone URL-Project-Github)

3. using Vite --> type in Terminal: create vite@latest .

4. select a framework react, select a variant jacascript

5. now run ##`npm install`

6. ##`npm run dev` to open on local server 3000

7. ##`npm install gh-pages --save-dev` (The command installs the gh-pages package as a development dependency for a Node.js project.)
   (DE:Installiert das Paket gh-pages als Entwicklungsabhängigkeit für ein Node.js-Projekt.)

8. go to package.json and add the following lines of code as a property: "homepage":`https://github.com/{username}/{repo-name}.git`, this is the link to your repo (you can copy it from the address bar on GitHub)

9. now add in package.json under "name", "private",
   "predeploy": "npm run build", "deploy": "gh-pages -d dist"
   (note: dist when using vite, build when using create-react-app)

10. go to vite.config.js and add under the plugins: the following lines of code
    base: '/name of the project'

11. type npm run deploy in Terminal to add to package.json File "deploy": "gh-pages -d dist",

- go to GitHub repo and refresh the page. now you should see 2 branches
- go to your repo and click on the settings button right next to "about"! then click on the checkbox "Use your GitHub Pages website" and apply your settings

These steps describe the process of creating, developing, and deploying a web application using React and Vite, as well as its deployment to GitHub Pages
