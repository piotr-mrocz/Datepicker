# Datepicker
My own datepicker. Created using Angular(TypeScript, HTML, CSS), Bootstrap.

How to use it:

1. Install Bootstrap:
  npm install bootstrap@next
  
2. Install Bootstrap Icons:
  npm i bootstrap-icons
  
3. Add style to angular.json:
  "styles": [
              "src/styles.css",
              "node_modules/bootstrap/dist/css/bootstrap.min.css",
              "node_modules/bootstrap-icons/font/bootstrap-icons.css"
  ],
  
  
4. Imports in app.module.ts:
  import { NgModule, LOCALE_ID } from '@angular/core';
  import { FormsModule } from '@angular/forms';
  import { DatepickerComponent } from './datepicker/datepicker.component';
  
  
  @NgModule({
  declarations: [
	DatepickerComponent,
  ],
  imports: [
    BrowserModule,
    FormsModule
  ],
  providers: [
    { provide: LOCALE_ID, useValue: 'pl-PL'} // set polish local
  ],
  bootstrap: [AppComponent]
  })
  export class AppModule { }
  
