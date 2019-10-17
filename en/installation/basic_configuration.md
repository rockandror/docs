# Basic Configuration

Once you have CONSUL running on the server, there are some basic configuration options that you probably want to define in order to start using it. To do this you will need to open your CONSUL installation through any internet browser and log in with the administration user \(initially it is the `admin@consul.dev` user with the password `12345678`\).

Once you have logged in you will see on the top right of the screen the "Admin" link that will take you to the administration interface. From this interface we recommend configuring the main basic options through the installation wizard, and once configured go through the other possible functionalities that can be desired by accessing the Configuration section from the Administration submenu.

## Installation Wizard
To access the Installation Wizard, in the side menu you will find the option "Configuration" and then the submenu "Wizards", where you can access the "Installation Wizard".

#### Step 1 - Welcome to the Consul installation wizard
In this wizard we will carry out step by step all the necessary configuration to be able to customize the application to the needs of your Institution. If you do not have any information requested in the wizard, you will be able to ignore it and modify it in the future in the related Settings Section or from this same Wizard.

#### Step 2 - Global Settings
In this step you can update some of the most important Global Application Settings. If you want to modify any of them once the Wizard has been carried out, you can go to the "Configuration > Global Configuration" section or by running the Installation Wizard again.

- Site name: This name will appear on mailers subject, help pages...
- Minimum age needed to participate: If you use a user verification system this will be the minimum age that users will be required to be. The user verification system will be discussed in more detail later. A new wizard has been included to configure the user verification system, which will be explained at the end of this section.

#### Step 3 - Participation processes
In this step you can activate/deactivate the participation processes that each Institution decides to use. If you want to modify any of them once the Wizard has been carried out, you can access the "Configuration > Participation Processes" section or by running the Installation Wizard again.

- Debates: The citizens' debate space is aimed at anyone who can present issues that concern them and about which they want to share their views with others.
- Proposals: Citizens' proposals are an opportunity for neighbours and collectives to decide directly how they want their society to be, after getting sufficient support and submitting to a citizens' vote.
- Number of supports necessary for approval of a Proposal: When a proposal reaches this number of supports it will no longer be able to receive more supports and is considered successful.
- Polls: Citizens' polls are a participatory mechanism by which citizens with voting rights can make direct decisions.
- Participatory budgeting: With participatory budgets, citizens decide which projects presented by their neighbours will receive a part of the budget.

#### Step 4 - Map configuration
In this step you will be able to activate/deactivate the geolocation of proposals and spending projects, and customize the way the map is shown to users. If you want to modify any of them once the Wizard has been carried out, you can access the "Configuration > Map Configuration" section or run the Installation Wizard again.
- Proposals and budget investments geolocation: Enables geolocation of proposals and investment projects.
- Latitude: Latitude to show the map position.
- Longitude: Longitude to show the position of the map.
- Zoom: Zoom to show the map position.

#### Step 5 - SMTP Connection
In this step you will be able to configure the SMTP connection to be able to send mails from the application. If you want to modify any of them once the Wizard has been carried out, you will be able to access the section "Configuration > SMTP Connection" or by running the Installation Wizard again.
- SMTP Configuration: Enable this feature to send emails through SMTP server.
- SMTP Host: Configure SMTP server host. Example: 'smtp.example.com'.
- SMTP Port: Configure SMTP server port. Example: 587.
- Domain: Configure SMTP server domain. Example: 'example.com'.
- SMTP User: Configure SMTP server user. Example: 'username'.
- SMTP Password: Configure SMTP server password. Example: 'password'.
- SMTP Authentication: Configure SMTP server authentication type. Example: 'plain'.
- Configure SMTP server TLS configuration. Example: 'true'

#### Step 6 - Languages and Time Zone
In this step you can set the default language of the application, the available languages and the time zone you are in. If you want to modify any of them once the Wizard has been carried out, you can go to the "Configuration > Regional Settings" section or by running the Installation Wizard again.
- Default locale: Define the default locale of the application using the selector that offers all available locales in the application.
- Application available locales: You will be able to see all the available locales in the application and enable/disable those that you consider appropriate.
- Time zone: Allows you to select the time zone in which you want to use the application.

#### Step 7 - Finish Wizard
If you want to modify any data once the Wizard has been carried out, you can modify it in the Configuration section or by running the Installation Wizard again.

At the end of the wizard will redirect us to the Configuration section where we can modify both the values entered and configure new features of the application not covered in this installation wizard explained in the following sections.

## Verification Wizard
To explain the use of this verification wizard we will explain step by step the content of each page of the wizard and at the end a section of examples of how to create verification processes using this wizard, which will be the perfect complement to correctly understand this functionality.

To access the Verification Wizard, in the side menu you will find the option "Configuration" and then the submenu “Wizards", where you will be able to access the "Verification Wizard".

#### Step 1 - Welcome to the verification process wizard
In this wizard we will carry out step by step all necessary configuration to be able to customize users verification process of the application to suite your verification needs.

To use the verification process that we are going to configure in this wizard you must activate:
- Customizable user verification process
and disable:
- Skip user verification

#### Step 2 - User verification methods
Enable or disable the available user verification methods you want. You can combine them to suite your needs.
- Verify a user against SOAP Remote Census
- Verify a user against the Local Census
- Verify a user's phone

Solo a los métodos de verificación habilitados les podremos asignar campos que crearemos en el siguiente paso. Asignar un campo a un método de verificación significa que ese campo le será enviado durante el proceso de verificación.

#### Paso 3 - Formulario de verificación de usuarios
En este paso podremos definir los campos que solicitaremos al usuario en el formulario de verificación. Y en los siguientes pasos podremos asignar cada uno de estos campos a uno o varios métodos de verificación.

El formulario para crear estos campos ofrece muchas posibilidades para permitir crear cualquier tipo de proceso de verificación.
- Etiqueta: El nombre con el que veremos el campo en el formulario de verificación de un usuario. Ofrece la posibilidad de añadir traducciones.
- Ayuda: Texto informativo que se mostrará al lado del campo que estamos definiendo. A este campo ayuda se le pueden dar diversos usos desde una descripción del campo hasta una definición del formato esperado.
- Nombre: Este es el nombre con el que guardaremos el campo en base de datos. El nombre es necesario que no contenga espacios en blanco y recomendable que este en minúsculas. En caso de ser un campo que se vaya a enviar al Censo Local, el nombre que definimos en este campo es el nombre con el que se intentará verificar el registro.
- Posición: Posición en la que mostraremos el campo en el formulario de verificación.
- Requerido: Marcar este checkbox obligará a rellenar el campo en el formulario. Si no se rellena en el formulario provocará un error de validación.
En caso de no marcarlo servirá para pedir información adicional que no queremos forzar a que el usuario lo introduzca para poder verificarse.
- Requiere campo de confirmación: Marcar este checkbox creará un campo adicional de confirmación. Si no se rellena con el mismo valor  provocará un error de validación. Este campo es útil cuando queremos asegurarnos de que el dato introducido es correcto, como por ejemplo podría ser el número de teléfono al que tenemos que enviar un código de confirmación.
- Visible: Por defecto este checkbox siempre esta marcado ya que la mayoria de los campos que creamos son para mostrarse en el formulario. Hay ciertos casos un poco específicos en los que podemos requerir crear campos que no necesariamente necesitan ser visibles en el formulario, como puede ser un campo del tipo "zona geográfica".
- Formato: En este campo se puede añadir una expresión regular para forzar un formato específico del valor introducido en el formulario de verificación. En caso de no cumplir con está expresión regular se provocará un error en la validación. Para el correcto funcionamiento de este campo es necesario introducir la expresión regular sin los escapados de inicio (/) y final(/). Si este campo se deja en blanco, no se aplica ningún validación de formato.
- Tipo del campo: En este selector se puede elegir que tipo de campo queremos crear:
  - Campo de texto
  - Campo checkbox: Permite forzar que el campo que vamos a crear sea de tipo checkbox y ofrece la posibilidad de añadirle un link asociado a este checkox. El caso más claro sería querer crear un checkox de terminos y condiciones de uso, que será necesario marcarlo para poder permitir la verificación y que queremos mostrar un link a una página de la aplicación donde se explican esos términos y condiciones de uso. Para utilizar correctamente este campo adicional se debe rellenar con el slug de una nueva página de nuestra aplicación, para ello debemos acceder a la sección de administración 'Contenido del sitio' > 'Personalizar páginas' y crear la página con el slug introducido.
  - Campo selector: Permite crear un campo del tipo selector y al seleccionarlo en el formulario de creación aparece un botón "Añadir nueva opción para el selector" que nos servirá para crear las opciones con sus respectivos valores que queremos que contenga nuestro selector, ofreciendo dos campos "Etiqueta" y "Valor" y la posibilidad de crear tantas opciones como necesitemos. Un ejemplo para este tipo de campo podría ser un selector para el tipo de documento, donde podríamos crear 2 opciones: (Etiqueta: DNI, valor 0) y (Etiqueta: Pasaporte, valor: 1).
  - Campo fecha

- Zona geográfica: Este checkox permite marcar un campo del tipo zona geográfica. Este campo se tendrá que asociar con el Censo Remoto y/o el Censo Local en los siguientes pasos. La finalidad de este campo es poder recuperar del Censo Remoto o del Censo local el dato referente a la zona geográfica y poder guardarlo directamente al usuario verificado. Este tipo de campo nos permitirá utilizar las funcionalidades de la aplicación referentes a la zona geográfica en la que se encuentra el usuario, como por ejemplo votar encuestas en función del distrito del usuario.

- Fecha de nacimiento: Esta checkox permite marcar un campo del tipo fecha de nacimiento. Este campo se tendrá que asociar con el Censo Remoto y/o el Censo Local en los siguientes pasos. La finalidad de este campo es poder recuperar del Censo Remoto o del Censo local la fecha de nacimiento y validar que el usuario verificado cumple la restricción de edad definida en la aplicación.


## Global configuration parameters

In the side menu you will find the option "Settings" and then the submenu "Global Settings". Here you will find many interesting parameters, but at the moment we recommend you to define some of the most basic ones. Later, when you are more familiar with the tool, you will be able to reconfigure other parameters:

* Site name. This name will appear in the subject of emails, help pages...
* Sender email name. This name will appear as the name of the sender in the emails sent from the application. As for example the email that the users receive to confirm that they have created their account.
* Sender email address. This email address will appear in the emails sent from the application.
* Main URL. Main URL of your website
* Minimum age needed to participate. If you use a user verification system this will be the minimum age that users will be required to be. The user verification system will be discussed in more detail later.
* Number of supports necessary for approval of a Proposal. If you use the citizen proposals section, you can define a minimum number of supports that the proposals need in order to be considered. Any user will be able to create proposals but only those that reach that value will be taken into account.
* Level x public official . CONSUL allows some user accounts to be marked as "official accounts" and their interventions on the platform are highlighted. This for example is used in a city if you want to define accounts for the Mayor, Councillors, etc. This public official option will allow you to define the official label that appears next to the user names of these accounts from most important \(level 1\) to least \(level 5\).

## Categories of proposals

When users create proposals on the platform, a few general categories are suggested to help organize the proposals. To define these categories you can go to the "Global Settings" menu and then to the "Proposal Topics" submenu. At the top you can write topics and create them with the button below.

## Definition of Geozones

Geozones are smaller territorial areas than the area in which you use CONSUL \(e.g. districts in a city in which CONSUL is used\). If the geozones are activated, it will allow for example that the citizen proposals are assigned to a specific area, or that the votings are restricted to people living in some area.

In the side menu you will find the option "Settings" and then the submenu "Manage geozones". To the right the button "Create geozone" will allow you to create new geozones. Only the name is necessary to define them, but you can add other data that are useful in certain sections. Initially we recommend that you start by defining only the names of the zones.

Once defined if you create a citizen proposal you will see how one of the options in the proposal creation form allows you to choose if your proposal refers to a specific geozone.

If you activate the geozones you can also display an image that represents the area with the zones. You can change this image in the "Global settings" menu in the "Customize images" submenu. The default image you can change is the one titled "map".

## Map to geolocate proposals

You can allow users to place proposals on a map when creating proposals. To do this you have to define which map you want to show.  
First go to the "Settings" menu and to the "Global Settings" submenu. There you will find three parameters that you will have to fill in:

* Latitude. Latitude to show the map position
* Length. Length to show the map position
* Zoom. Zoom to show the position of the map. You can try an initial value and then change it later.

At the top of this page you will find three tabs: "Configuration settings", "Features", "Map configuration". Now go to the second tab "Features".

On this page you will find one of the functionalities titled "Proposals and budget investments geolocation ". The message "Functionality enabled" should appear on your right. If not, click on the "Enable" button.

Then, at the top of this page, go to the "Map configuration" tab. If everything has been configured correctly you will see here the map centered on the latitude and longitude you entered before. You can correctly center the map and change the zoom level directly on the map by clicking on the "Update" button below it.

## Emails to users

CONSUL sends a series of emails to users by default. For example when creating a user account, trying to recover a password, receiving a message from another user, etc.

All emails sent can be viewed in the menu "Messages to users" in the submenu "System Emails". There you will be able to preview each email and see the file where the content of the email is in case you want to change it.

## Basic information pages

CONSUL has a number of basic information pages that will be shown to users, e.g. "Privacy Policy", "Frequently Asked Questions", "Congratulations you have just created your user account", etc.

You can see the pages that exist by default and modify them in the menu "Site Content" in the submenu "Custom Pages".

## Main page of the site

When users open your CONSUL installation they will see the home page of the platform. This page is fully configurable, so that you can show the content that seems most relevant to you. You can modify it from the menu "Site content" in the submenu "Homepage".

Try creating "Headers" and "Cards" and activating the different functionalities you will find below to see the effect they have on your homepage.

## Platform texts

If you access the menu "Site content" and the submenu "Custom information texts" you will see different tabs with a series of texts. These are all the texts displayed on the platform. By default you can use the existing ones, but at any time you can access this section to modify any of the texts.

For more information on how to add new translations to your version of CONSUL access the "Texts and translations" section of this documentation.

## Channels of participation

By default you will find in CONSUL different ways of participation for users. To begin with and familiarise yourself with the tool, we recommend that you have all of them activated, but you can deactivate the ones that do not seem necessary to you. To do this, go to the "Settings" menu and then to the "Global Settings" submenu. At the top of this page you will find three tabs: "Configuration settings", "Features", "Map configuration". Go to the second tab "Features".

You will find different functionalities with the names of the different participation channels "Debates", "Proposals", "Voting", "Collaborative Legislation" and "Participatory Budgets". You can deactivate any of the functionalities and it will no longer be shown in your CONSUL installation.

### More information and detailed documentation

These options above will allow you to have a basic version of CONSUL to start using. We recommend that you access the [CONSUL Documentation and Guides](../getting_started/documentation_and_guides.md) section where you can find more detailed documentation.
