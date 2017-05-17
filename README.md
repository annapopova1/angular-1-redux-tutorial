<strong>tl;dr:</strong><br/>
	Install:<br/>
	1 - Clone the repository to a local folder;<br/>
	2 - Run the command "npm install" on the root of each project steps;<br/>
	3 - Run the command "gulp" for either one of the steps you want to run;<br/>
<br/>
	Now opening your browser and pointing to http://localhost:3000 should show you the app running.<br/>
<br/>

<strong>More detailed:</strong>	
<br/>
Step 1 - Empty project:<br/>
	1 This step will only show how to get a copy of the initial project and run it on your local machine;<br/>
	2 First you will need to have both NPM and Git configured on your local machine, this instalation is out of the scope of this tutorial but there are tons of tutorials on how to do this on the Internet;<br/>
	3 Open your command line and navigate to the location where you want to add the tutorial;<br/>
	4 Now clone the repository to your local machine by using the following GIT command:<br/>
		"git clone https://github.com/pentaho-arua/angular-1-redux-tutorial.git"<br/>
	5 Now you should have the entire project on your local machine<br/>
	6 To check the first step open the folder named "step-1" on your favorite code editor or IDE, if you're using Visual Studio Code you can navigate to "step-1" folder and execute the command "code ." and the project will open on VSC;<br/>
	7 In order to be able to run the application with need to install the dependencies using NPM. To do so you need to run the following command on the root folder of "step-1":<br/>
		"npm install"<br/>
	8 Now since we are using gulp and babel in the project we only need to use the "gulp serve" command to start the server;<br/>
	9 Open your browser and navigate to "localhost:3000" and you will see the application runing. At this time you will simply have a menu with Home and a small text at the center of the screen saying "This is the Homepage of our simple Angular app";<br/>
<br/>
Step 2 - To-do App with Angular only:<br/>
	1 This step will show a working To do app using only Angular;<br/>
	2 To run this step simply do the same steps done on step-1 starting from point 6;<br/>
	3 Now you can see that there is a new menu called noredux and by clicking on it you can interact with the simple To-do app;<br/>
	4 To achieve this we created a new component named "noredux";<br/>
	5 On the app.js file we added the reference to the new component and the needed code so that if would be possible to navigate to it;<br/>
	6 On the navigation component we changed the file navigation.html to also show the noredux menu right next to the Home;<br/>
<br/>
Step 3 - To-do App using Angular, Redux (ng-redux), Selectors and async actions using thunk:<br/>
	1 To run this step simply do same as done on the previous steps;<br/>
	2 Several dependencies were added to the project, such as ng-redux and redux-thunk;<br/>
	3 A new component called WithRedux was created and references were added to the app.js;<br/>
	4 A new menu was also created to the navigation.html file for the WithRedux component;<br/>
	5 Several new folders were created in order to separate files to be used for redux:<br/>
		- actions:<br/>
			- This is were the todo actions are stored;<br/>
		- reducers:<br/>
			- Here you have the todo reducer that will handle the state of the todo app;<br/>
		- selectors:<br/>
			- Some helper functions there are used for the selectors;<br/>