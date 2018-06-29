#Truenorth Setup

1. Pull the latest [TrueNorth App](https://emmersionlearning.visualstudio.com/EmmersionLearning/_git/TrueNorth).

---

(Commands to remove the previous library, No need to do if fresh clone from repository)

1.  Execute a `npm uninstall angular-2-data-table` command.
2.  Execute a `rm -rf node_modules/angular-2-data-table` command.

---

3. First, you need to connect to angular-tn-data-table feed by doing that you have to install first 'vsts-npm-auth':
   - `npm install -g vsts-npm-auth --registry https://registry.npmjs.com --always-auth false`
4. Configure your local to have vsts authentication:
   - `vsts-npm-auth -config .npmrc`
   (at this point, Microsoft Authentication will ask for your credentials.)
4. Once your authentication is successful, Execute npm install command:
   - `npm install` 

For references check this [docs](https://docs.microsoft.com/en-us/vsts/package/npm/npmrc?view=vsts)

###To make sure everything is working fine

Execute this command (this will ensure that you got the right library and is built and packaged well by webpack.) :
 - `node node_modules/webpack/bin/webpack.js` 

###Pro Tip

- if you encountered weird issues, such as still referencing angular-2-data-table during the execution of 'node node_modules/webpack/bin/webpack.js' command,
  kindly check the node_modules folder in "C:/<username>/", and make sure angular-2-data-table is removed.

#Contributing

1. Pull the latest code for [angular-tn-data-table](https://emmersionlearning.visualstudio.com/EmmersionLearning/_git/TrueNorth.AngularDataTable)
2. Follow the TrueNorth [GIT Guidelines and Standards](/Development-Guidelines-and-Standards/GIT-Guidelines-and-Standards)
3. Push your updates in this repository, get someone to take a look at it.
4. Once verified and tested, increment the version in package.json file.(e.g. 0.1.3 -> 0.1.4)
5. Then do a `npm publish` command.

#Truenorth TestTaker/Admin App updates on the library

v0.1.2: updated a behavior to attach a mouse-click event to score report section.
v0.1.3: configured to become a package feed in vsts.
v0.1.4: updated installation and readme documents

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
