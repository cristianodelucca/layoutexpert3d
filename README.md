## See it

This repository includes an example application built using blueprint3d:

### http://furnishup.github.io/blueprint3d/example/

## What is this?

This is a customizable application built on three.js that allows users to design an interior space such as a home or apartment. Below are screenshots from our Example App (link above). 

1) Create 2D floorplan:

![floorplan](https://s3.amazonaws.com/furnishup/floorplan.png)

2) Add items:

![add_items](https://s3.amazonaws.com/furnishup/add_items.png)

3) Design in 3D:

![3d_design](https://s3.amazonaws.com/furnishup/design.png)

## Get started

To get started, run:

    npm update
    npm run-script build

The latter command generates `build/blueprint3d.js` and also copies it to `example/js`

## /src directory

The `src` directory contains the core of the project. Here is a description of the various sub-directories:

`floorplanner` - 2D view/controller for editing the floorplan

`items` - Various types of items that can go in rooms

`model` - Data model representing both the 2D floorplan and all of the items in it

`three` - 3D view/controller for viewing and modifying item placement

`utils` - some shared functions that are mostly deprecated in favor of functionality provided by various npm modules

## License

This project is open-source! See LICENSE.txt for more information.

## TODO

This project requires a lot more work. In general, it was rushed through various prototype stages, and never refactored as much as it probably should be. Here are some things that clearly need attention:

- Better documentation
- Test suite
- Make it easier to build a complete application using blueprint3d (cleaner API, more inclusive base, easier integration with a backend)
- Better serialization format for saving/loading "designs"
- Remove the dependency on jquery from the core source!
- Better use of npm conventions and packaging
- Various bug fixes
