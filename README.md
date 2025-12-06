# BusStationACAD
Faculty project of "Universitate" bus station located in Bucharest made in AutoCAD

# CAD Project: 3D Bus Stop Model

<div align="center">

![Status](https://img.shields.io/badge/Maintained%3F-no-red.svg?style=flat-square)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)
![Repo Size](https://img.shields.io/github/repo-size/dbogdanm/BusStationACAD?style=flat-square)

<br/>

![AutoCAD](https://img.shields.io/badge/AutoCAD-0696D7?style=for-the-badge&logo=autodesk&logoColor=white)
![Drafting](https://img.shields.io/badge/Skill-2D%20Drafting-lightgrey?style=for-the-badge)
![Design](https://img.shields.io/badge/Design-Architecture-orange?style=for-the-badge)

</div>

This repository contains a 3D model of a modern bus stop, created as a project for the "Computer-Aided Design" course at the University of Bucharest. The primary focus was on the technical execution and 3D modeling process using Autodesk AutoCAD.

## Academic Context

* **Institution:** University of Bucharest
* **Faculty:** Faculty of Mathematics and Informatics
* **Program:** Computer Science and Information Technology
* **Course:** Computer-Aided Design (Proiectare Asistată de Calculator)
* **Student:** Dinu Bogdan-Marius
* **Coordinator:** Prof. Drăgan Mihăiță

## Technical Summary & Modeling Workflow

The entire project was developed in Autodesk AutoCAD, adhering to a 1:1 scale with centimeters as the working unit. The core methodology involved a hybrid 2D-to-3D and direct 3D modeling approach.

### 1. 2D-to-3D Extrusion
The most common workflow was to first create precise 2D profiles and then give them depth.
* **2D Drafting:** Profiles for components like the roof, bench, and waste receptacle were drawn using `Line` , `Offset` (e.g., 2cm for bench planks and receptacle walls), and `Arrayrect` (for repetitive elements like road markings).
* **3D Extrusion:** The `Presspull` command was used extensively to extrude these 2D shapes into 3D solids.

### 2. Direct 3D Modeling
Complex components were modeled directly using 3D primitives.
* **Primitives Used:** `Box` , `Cylinder` , `Sphere` , and `Cone`.
* **Boolean Operations:** The `Subtract` command was used to create hollow shapes, such as the inner part of the waste bin and the luminaire housing.

### 3. Assembly and Modification
Components were positioned and adjusted using standard transformation tools.
* **Manipulation:** `Move` was used for assembly, `Scale` to resize elements like trees, and `Arraypolar` to create circular patterns (e.g., camera LEDs).
* **Organization:** The `Layer` command was used from the beginning to organize components and manage properties.

### 4. Visualization
Basic materials and textures were applied for realism.
* **Materials:** The `Mat` command was used to apply textures from the library or external files (e.g., photovoltaic cells, leaves, bark, road surfaces).
* **Decals:** The `Attach` command was used to apply 2D images, like the recycling logo and bus stop sign, onto 3D faces.

## Component Modeling Breakdown

* **Roof:** Started as a 170x380cm 2D rectangle (`Line`) , then extruded to a 20cm height using `Presspull`. `Text` was added and positioned with `Move`.
* **Bench:** A detailed 2D side-profile was drawn (`Line`). Planks were defined using `Offset` (2cm) and the entire profile was extruded with `Presspull`.
* **Surveillance Camera:** Modeled directly in 3D. The main body is a `Cylinder` , with a `Cone` and `Sphere` forming the lens assembly. A circular pattern of spheres (`Arraypolar`) simulates the IR LEDs. The mounting arm and hood were also modeled as 3D solids.
* **Road & Sidewalk:** `Line` defined the lane edges. The bus bay was created with `Line` at a 45° angle. The curb was generated with `Offset` (20cm). The "zig-zag" marking was drawn with `Line` commands based on a 30° angle. The `BUS` lettering was added with `Text`. All 2D geometry was converted to 3D with `Presspull`.
* **Decorative Trees:** The trunk and branches were modeled as pyramids with an octagonal base. A single leaf was modeled using `Line` and `Presspull` , then duplicated and distributed using `Arraypolar` and `Copy-Paste`.

## Project Gallery

![image alt](https://github.com/dbogdanm/BusStationACAD/blob/main/statie1.png?raw=true)
![image alt](https://github.com/dbogdanm/BusStationACAD/blob/main/statie2.png?raw=true)
![image alt](https://github.com/dbogdanm/BusStationACAD/blob/main/statie3.png?raw=true)
 More project photos can be found in the documentation.
