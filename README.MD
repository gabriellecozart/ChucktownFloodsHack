This is a project created for the Chucktown Floods Hack Agenda.

# Requirements

This projects used Ionic.
Install by running:
`npm install -g ionic corova`

After cloning the repository, run `npm install`.

# Start Development

To start the webserver run `ionic serve` inside the project directory.

# How to add a new page

To add a new page run `ionic g page page_name`

Add an import to the `home.ts` file:

`import {Page_Name} from '../page_name/page_name';`

And then add `page_name = Page_Name;` to the HomePage constructor.

Finally to add a button leading to the page add this line to the home.html:

`<button [navPush]="page_name">Go To Page_Name</button>`

In case the ubtton does not work open up `app/app.module.ts` and add
`Page_Name` to `NgModule.declarations` and `NgModule.entryComponents'.
