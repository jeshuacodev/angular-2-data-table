#Truenorth Setup

- pull the latest TrueNorth App [source code](https://emmersionlearning.visualstudio.com/EmmersionLearning/_git/TrueNorth).

---

(To remove the previous library, No need to do if fresh clone from repository)

- execute a 'npm uninstall angular-2-data-table' command.
- execute a 'rm -rf node_modules/angular-2-data-table' command.

---

- execute a 'npm install angular-tn-data-table' command

##To make sure everything is working fine

- execute a 'node node_modules/webpack/bin/webpack.js' command, this will ensure that you got the right library and
  is built and packaged well by webpack.

##Pro Tip

- if you encountered weird issues, such as still referencing angular-2-data-table during the execution of 'node node_modules/webpack/bin/webpack.js' command,
  kindly check the node_modules folder in "C:/<username>/", and make sure angular-2-data-table is removed.

#Contributing

- pull the latest code for [angular-tn-data-table](https://emmersionlearning.visualstudio.com/EmmersionLearning/_git/TrueNorth.AngularDataTable)
- follow the TrueNorth [GIT Guidelines and Standards](/Development-Guidelines-and-Standards/GIT-Guidelines-and-Standards)
- push your updates in this repository, get someone to take a look at it.
- once verified and tested, increment the version in package.json file.(e.g. 0.1.3 -> 0.1.4)
- then do a 'npm publish' command.

#Truenorth TestTaker/Admin App updates on the library

- updated a behavior to attach a mouse-click event to score report section.

#Author's Docs

## Angular 2 Data Table

### ** Updated for Angular 5 [here](https://github.com/ggmod/angular-5-data-table). This repo will not be updated **

A simple Angular 2 data table, with built-in solutions for features including:

- pagination
- sorting
- row selection (single/multi)
- expandable rows
- column resizing
- selecting visible columns

The component can be used not just with local data, but remote resources too: for example if the sorting and paging happen in the database.

The templates use bootstrap CSS class names, so the component requires a bootstrap .css file to be present in the application using it.

Check out the [demo](https://ggmod.github.io/angular-2-data-table-demo) and its [code](https://github.com/ggmod/angular-2-data-table-demo) for examples of how to use it.

## Installing:

`npm install angular-2-data-table --save`

#### Licensing

MIT License
