# BusStationACAD
Faculty project of "Universitate" bus station located in Bucharest made in AutoCAD

# CAD Project: 3D Bus Stop Model

![AutoCAD](https://img.shields.io/badge/Software-AutoCAD-blue.svg)

This repository contains a 3D model of a modern bus stop, created as a project for the "Computer-Aided Design" course at the University of Bucharest. The primary focus was on the technical execution and 3D modeling process using Autodesk AutoCAD.

## Academic Context

* **Institution:** University of Bucharest
* **Faculty:** Faculty of Mathematics and Informatics
* **Program:** Computer Science and Information Technology
* **Course:** Computer-Aided Design (Proiectare Asistată de Calculator)
* **Student:** Dinu Bogdan-Marius
* **Coordinator:** Prof. Drăgan Mihăiță

## Technical Summary & Modeling Workflow

[cite_start]The entire project was developed in Autodesk AutoCAD, adhering to a 1:1 scale with centimeters as the working unit[cite: 63]. The core methodology involved a hybrid 2D-to-3D and direct 3D modeling approach.

### 1. 2D-to-3D Extrusion
The most common workflow was to first create precise 2D profiles and then give them depth.
* [cite_start]**2D Drafting:** Profiles for components like the roof, bench, and waste receptacle were drawn using `Line` [cite: 69, 91, 102][cite_start], `Offset` (e.g., 2cm for bench planks and receptacle walls) [cite: 92, 102][cite_start], and `Arrayrect` (for repetitive elements like road markings)[cite: 142].
* [cite_start]**3D Extrusion:** The `Presspull` command was used extensively to extrude these 2D shapes into 3D solids[cite: 72, 92, 105, 153].

### 2. Direct 3D Modeling
Complex components were modeled directly using 3D primitives.
* [cite_start]**Primitives Used:** `Box` [cite: 110, 135, 171][cite_start], `Cylinder` [cite: 111, 122, 128][cite_start], `Sphere` [cite: 128, 187][cite_start], and `Cone`[cite: 186].
* [cite_start]**Boolean Operations:** The `Subtract` command was used to create hollow shapes, such as the inner part of the waste bin [cite: 110] [cite_start]and the luminaire housing[cite: 128].

### 3. Assembly and Modification
Components were positioned and adjusted using standard transformation tools.
* [cite_start]**Manipulation:** `Move` [cite: 75, 128, 166, 174, 200] [cite_start]was used for assembly, `Scale` [cite: 255] [cite_start]to resize elements like trees, and `Arraypolar` to create circular patterns (e.g., camera LEDs)[cite: 188].
* [cite_start]**Organization:** The `Layer` command was used from the beginning to organize components and manage properties[cite: 69].

### 4. Visualization
Basic materials and textures were applied for realism.
* [cite_start]**Materials:** The `Mat` command was used to apply textures from the library or external files (e.g., photovoltaic cells, leaves, bark, road surfaces)[cite: 135, 161, 232].
* [cite_start]**Decals:** The `Attach` command was used to apply 2D images, like the recycling logo and bus stop sign, onto 3D faces[cite: 116, 123].

## Component Modeling Breakdown

* [cite_start]**Roof:** Started as a 170x380cm 2D rectangle (`Line`) [cite: 69][cite_start], then extruded to a 20cm height using `Presspull`[cite: 72]. [cite_start]`Text` was added and positioned with `Move`[cite: 75].
* [cite_start]**Bench:** A detailed 2D side-profile was drawn (`Line`)[cite: 91]. [cite_start]Planks were defined using `Offset` (2cm) [cite: 92] [cite_start]and the entire profile was extruded with `Presspull`[cite: 92].
* [cite_start]**Surveillance Camera:** Modeled directly in 3D[cite: 185]. [cite_start]The main body is a `Cylinder` [cite: 186][cite_start], with a `Cone` and `Sphere` forming the lens assembly[cite: 186, 187]. [cite_start]A circular pattern of spheres (`Arraypolar`) simulates the IR LEDs[cite: 188]. [cite_start]The mounting arm and hood were also modeled as 3D solids[cite: 189].
* [cite_start]**Road & Sidewalk:** `Line` defined the lane edges[cite: 142]. [cite_start]The bus bay was created with `Line` at a 45° angle[cite: 144]. [cite_start]The curb was generated with `Offset` (20cm)[cite: 146]. [cite_start]The "zig-zag" marking was drawn with `Line` commands based on a 30° angle[cite: 164, 165]. [cite_start]The `BUS` lettering was added with `Text`[cite: 166]. [cite_start]All 2D geometry was converted to 3D with `Presspull`[cite: 153].
* [cite_start]**Decorative Trees:** The trunk and branches were modeled as pyramids with an octagonal base[cite: 214]. [cite_start]A single leaf was modeled using `Line` and `Presspull` [cite: 220][cite_start], then duplicated and distributed using `Arraypolar` and `Copy-Paste`[cite: 226].

## Project Gallery

![image alt](https://github.com/dbogdanm/BusStationACAD/blob/main/statie1.png?raw=true)
![image alt](https://github.com/dbogdanm/BusStationACAD/blob/main/statie2.png?raw=true)
![image alt](https://github.com/dbogdanm/BusStationACAD/blob/main/statie3.png?raw=true)
 More project photos can be found in the documentation.
