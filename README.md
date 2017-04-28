# Start the App

```
npm install -g @angular/cli
npm install
ng serve
```

# Full tutorial
Install Angular CLI

```
npm install -g @angular/cli
```

Create a new app with angular CLI
```
ng new angular-material-seed
cd angular-material-seed
```


Install Angular Material and Angular Animations
```
npm install --save @angular/material @angular/animations
```

App Module dependencies to app/app.module.ts

```
import {BrowserAnimationsModule} from '@angular/platform-browser/animations';
import {MdIconModule, MdInputModule, MdToolbarModule, MdMenuModule, MdButtonModule, MdCardModule} from '@angular/material';


BrowserAnimationsModule,
MdIconModule,
MdInputModule,
MdToolbarModule,
MdMenuModule,
MdButtonModule,
MdCardModule
```


Design a very basic and simple html in app.component.html
```
<div>
  <md-toolbar color="primary">
    <span><md-icon></md-icon></span>

    <span>{{title}}</span>

    <button md-icon-button [md-menu-trigger-for]="menu">
      <md-icon>more_vert</md-icon>
    </button>
  </md-toolbar>

  <md-menu x-position="before" #menu="mdMenu">
    <button md-menu-item>Option 1</button>
    <button md-menu-item>Option 2</button>
  </md-menu>

  <md-card>
    <md-card-content>
    <form class="example-form" layout-align="center">
      <md-input-container>
        <input mdInput placeholder="Name">
      </md-input-container>
      <md-input-container>
        <input mdInput placeholder="City">
      </md-input-container>
    </form>
    </md-card-content>
    <md-card-actions>
      <button md-fab>
        <md-icon>check circle</md-icon>
      </button>
    </md-card-actions>
  </md-card>

</div>
```


Import a basic style in app/styles.css
```
@import '~@angular/material/prebuilt-themes/indigo-pink.css';
```

Add Icons reference in index.html
index.html
```
<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
```

Start the application
```
ng serve
```


Links
https://material.angular.io



