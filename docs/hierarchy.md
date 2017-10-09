# React Component Hierarchy

The app will follow a standard VR component hierarchy:

File Structure:
* `Components`
  + `Scenes` Each scene owns a Pano image
    - `Layouts` Flexbox styling for the elements of a scene
      - `Elements` Smaller components such as tables and buttons

## Functional Component hierarchy

* `Root`
  + `App`
    - `Switch` with `Routes` for all other components

## Title Scene

* `TitleScene`
  + Route: `/#/title`
  + State: none
  + Components:
    - `Pano`
    - `TitleLayout`
      - `Title`
      - `Button` continues to Dashboard Scene

## Dashboard Scene

* `DashboardScene`
  + Route:
  + State:
  + Components:
    - `Pano`
    - `DashboardLayout`
      - `DashboardButtons`
      - `Button` enters a Phobia Scene

## Phobia Scene

There will be four of these scenes, each structured as follows:

* `PhobiaScene`
  + Route:
  + State:
  + Components:
    - `Pano`
    - `PhobiaLayout`
      - `Phobia`
      - `Button` back to Dashboard
