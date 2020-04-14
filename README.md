# AtlasDemo

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 9.0.5.

Here is a guide on how to use Phoenix Library for building an event display application.

## Create an Angular application
[Set up the environment](https://github.com/emiliocortina/atlas-demo.git) and create a default angular application with

    ng new app-name --style=scss --routing=true

## Install library dependencies

    npm i three dat.gui @tweenjs/tween.js @angular/animations @angular/cdk @angular/material

## Install Phoenix library

    npm i phoenix-library

## Import Phoenix Library

In your src/app/app.module.ts, at the top add the following import:

    import {PhoenixLibraryModule} from 'phoenix-library';

And add that module to the imports array declarations:

    imports: [
        BrowserModule,
        AppRoutingModule,
        PhoenixLibraryModule
    ]

## Import Phoenix styles

In your src/styles.scss, add:

    @import "~phoenix-library/index.scss";

## Use Phoenix components

Now you are all set to use the library components on your app.
Start by replacing the content of your src/app/app.component.html with the following:

    <phoenix-experiment-info experiment="atlas"></phoenix-experiment-info>
    <phoenix-ui-menu></phoenix-ui-menu>
    <phoenix-event-display></phoenix-event-display>

Note that you can remove the experiment-info component if you don't want to display an overlay with the experiment logo.