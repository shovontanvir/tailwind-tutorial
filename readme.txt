Initializing a New Project: 
1)	Setting Up Development Environment:
a)	Create a folder:
In your PC create an empty folder and name it according to the project name.
b)	Setting up git:
	Check git version [git  --version]
	Config git [git config –global user.name “user name of your git account” & git config –global user.email “email address of your git account”]
	Initialize the folder as a local git repository [git init]
	Link online repository with the local repository [git remote add origin “url of the remote repository”]
c)	Setting up node.js and npm: 
a.	Check versions [node -v & npm -v]
b.	Initialize npm [npm init  -y]
d)	Install lite-server for real time evaluation:
	Install lite-server as developer dependency [npm install lite-server –save-dev]
	Inside package.json file update the scripts 
“scripts”: {
“start”: “npm run lite”,
“task”: “whatever it has, leave it as it is”,
“lite”: “lite-server”
}
e)	Installing TailwindCSS : 
	Install tailwindcss [npm I -D tailwindcss]
	Install plugin in VScode for TailwindCSS [tailwindcss intelllisense] 
	Create a config file for tailwind css [npx tailwindcss init]
	Create two folders named src and output in the root directory
	In the src folder create a file named tailwind.css
o	@tailwind base;
o	@tailwind components;
o	@tailwind utilities;
	Create a folder named .vscode
	Create a file inside .vscode folder named settings.json
{
“css.validate’: false;
“tailwindCSS.emmetCompletions”: true;
}

