# Angular-Basic-Commands

# Update Angular CLI
  npm install -g @angular/cli
  
# Create Angular Project
  ng new ProjectName
  
# Run Angular Project
  ng serve 
  
# Create a New Component 
  ng generate component ComponentName
  
# Add NPM Package 
  npm install --save PackageName
  
# Add Angular Material 
  npm install --save @angular/material
  or 
  ng add @angular/material

# how to add html template to angular application
https://www.kindsonthegenius.com/how-to-integrate-admin-lte-with-angular/

# always add Css and Scripts into angular.json files (below example is of admin lte template)

    
    "scripts": [
              "src/assets/plugins/jquery/jquery.min.js",
              "src/assets/plugins/jquery-ui/jquery-ui.min.js",
              "src/assets/plugins/bootstrap/js/bootstrap.bundle.min.js",
              "src/assets/plugins/chart.js/Chart.min.js",
              "src/assets/plugins/sparklines/sparkline.js",
              "src/assets/plugins/jqvmap/jquery.vmap.min.js",
              "src/assets/plugins/jqvmap/maps/jquery.vmap.usa.js",
              "src/assets/plugins/jquery-knob/jquery.knob.min.js",
              "src/assets/plugins/moment/moment.min.js",
              "src/assets/plugins/daterangepicker/daterangepicker.js",
              "src/assets/plugins/tempusdominus-bootstrap-4/js/tempusdominus-bootstrap-4.min.js",
              "src/assets/plugins/summernote/summernote-bs4.min.js",
              "src/assets/plugins/overlayScrollbars/js/jquery.overlayScrollbars.min.js",
              "src/assets/dist/js/adminlte.js",
              "src/assets/dist/js/pages/dashboard.js"
    ]
    
    "styles": [
              "src/styles.css",
              "src/assets/plugins/fontawesome-free/css/all.min.css",
              "src/assets/plugins/tempusdominus-bootstrap-4/css/tempusdominus-bootstrap-4.min.css",
              "src/assets/plugins/icheck-bootstrap/icheck-bootstrap.min.css",
              "src/assets/plugins/jqvmap/jqvmap.min.css",
              "src/assets/dist/css/adminlte.min.css",
              "src/assets/plugins/overlayScrollbars/css/OverlayScrollbars.min.css",
              "src/assets/plugins/daterangepicker/daterangepicker.css",
              "src/assets/plugins/summernote/summernote-bs4.min.css"

    ],
    
# App Routing Example

      import { NgModule } from '@angular/core';
      import { RouterModule, Routes } from '@angular/router';
      import { LoginComponent } from './login/login.component';

      const routes: Routes = [
        { path:'', redirectTo: '/login', pathMatch:'full' }, //path match full it takes the base url else it will get confuse
        { path:'login', component: LoginComponent}
      ];

      @NgModule({
        imports: [RouterModule.forRoot(routes)],
        exports: [RouterModule]
      })
      export class AppRoutingModule { }


# Angular Forms and Form Validations
https://www.bezkoder.com/angular-10-form-validation/
