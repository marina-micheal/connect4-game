# Connect4 Game
A mini game written in Java, to practice OOP.

## Idea

"Fantastic Four" will be a upgraded version of the classis "Connect Four" game. Two players can each in return select a column where they want to drop a chip in there represented colour.To be the first player to connect 4 of the same colored discs in a row (either vertically, horizontally, or diagonally)


## UML class diagram

The software architecture of this game follows the MVC (model, view, controller) concept, where the programm logic is separated from the GUI (graphical user interface). The controller unit is the manages the information exchange between the modul (containing the game objects), and the view (representing the GUI, incl. GUI objects).

![UML_class_diagram](images/Capture.JPG "UML class diagram")
![UML_class_diagram](images/uml1.jpg "UML class diagram")
![UML_class_diagram](images/uml1.png "UML class diagram")
![UML_class_diagram](images/uml2.png "UML class diagram")
![UML_class_diagram](images/uml3.png "UML class diagram")
![UML_class_diagram](images/uml4.png "UML class diagram")
![UML_class_diagram](images/uml5.png "UML class diagram")
updated version: https://miro.com/app/board/o9J_lHxQrZg=/

## Rules of the Game

Two players can each in return select a column where they want to drop a chip in there represented colour. The chip will be placed in the last empty row of that column. If a field in a column is taken, the following chip will be placed in the row above this field in the same column. 

## GUI Mockup

Using Scene Builder a first GUI design is proposed. Based on this [FXML file]
![GUI_Design_v1](images/welcome.JPG.JPG "Fantastic Four GUI Design from Scene Builder")
![GUI_Design_v1](images/2-menu.JPG "Fantastic Four GUI Design from Scene Builder")
![GUI_Design_v1](images/3-user1.JPG "Fantastic Four GUI Design from Scene Builder")
![GUI_Design_v1](images/4-user2.JPG "Fantastic Four GUI Design from Scene Builder")
![GUI_Design_v1](images/5-gameboard.JPG "Fantastic Four GUI Design from Scene Builder")
![GUI_Design_v1](images/6-won.JPG "Fantastic Four GUI Design from Scene Builder")
![GUI_Design_v1](images/7-account.JPG "Fantastic Four GUI Design from Scene Builder")
![GUI_Design_v1](images/8-help.JPG "Fantastic Four GUI Design from Scene Builder")

## How to get it running on your machine
 * Install JAVA and JavaFX libraries
 * Add JAVA_HOME to Windows environment variables
 * set PATH_TO_FX="path\to\javafx-sdk-15.0.1\lib"
 * In IntelliJ, configure the project
 * Configuring the project structure
	* Select File --> Project Structure --> Project --> Select Java JDK 16
	* Select File --> Project Structure --> Libraries --> Add JavaFX libraries to list of libraries
 * Configuring the Run Configurations
	* Select menu Run --> Edit Configurations
	* Add new configuration --> Application
		* In the application configuration, defined the application name
		* Select "Build and Run" --> Java version 16
		* Select Main class from 
		* Add the following line to the VM configurations
		* Run --> Edit Configurations --> Check VM Options from "Modify Options"
		```
		--module-path "C:\Program Files\Java\jdk-16\javafx-sdk-16\lib" --add-modules javafx.controls,javafx.fxml
		```
