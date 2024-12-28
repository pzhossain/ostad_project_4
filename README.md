<H1> Project Requerment</H1>

<H2>### Project Features:</H2>

Add, edit, and delete vehicles.
Save data in a JSON file.
Display vehicle details in a Bootstrap card layout.


<H2>### Project Files and Folders Structure:</H2>

project/
├── app/
│   └── Classes/
├── data/
│   └── vehicles.json
├── public/
│   ├── index.php
│   └── views/
│       ├── add.php
│       ├── edit.php
│       ├── delete.php
│       ├── header.php


<H2>### Core Implementation:</H2>

* Trait: Create a FileHandler trait to handle JSON file operations:
Reading from the vehicles.json file.
Writing to the vehicles.json file.

* Interface: Define a VehicleActions interface with the following methods:
addVehicle($data)
editVehicle($id, $data)
deleteVehicle($id)
getVehicles()


* Abstract Class: Create an abstract VehicleBase class to handle shared vehicle properties (name, type, price, image) and define an abstract method:
getDetails()


* Concrete Class: Implement the VehicleManager class:
Use the FileHandler trait.
Extend the VehicleBase class.
Implement the VehicleActions interface.
