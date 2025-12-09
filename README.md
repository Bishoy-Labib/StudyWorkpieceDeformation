# Workpiece Deformation

## 1. Introduction
[cite_start]The research includes a study on workpiece deformation due to fixturing, as clamping forces affect the geometrical accuracy and the quality during the manufacturing process[cite: 127]. [cite_start]The problem appears after machining, once the clamping forces are released, the material will return to its original shape and the newly machined flat surface will be concaved, resulting geometrical inaccuracy[cite: 132].

[cite_start]The workpiece deformation can be avoided or set to minimum by using appropriate clamping methods and parameters[cite: 133].

## 1.2.1. Methods
* [cite_start]**Analytical Approach:** The analytical approach is used to calculate the theoretical amount of clamping force applied by the vice on the workpiece for different torques[cite: 141].
* [cite_start]**Experimental Approach:** The experimental approach is carried out a set of measurements setups done with the Coordinate Measuring Machine for different workpieces to determine the behavior of the workpieces due to clamping and the amount of deformation[cite: 143].
* [cite_start]**Computer Aided Engineering Approach:** The CAE approach will carry out simulation using FEM techniques using ANSYS to simulate the deformation of the workpiece due to clamping and later compare these results to the measured results[cite: 145].

## 3. Workpiece Preparation
[cite_start]The workpieces were made of aluminum alloy 6082 (AlMgSi1) bars with a square cross section 20x20 [mm] and 40x40 [mm][cite: 714]. [cite_start]The Gerardi StandardFLEX vise was used with 24mm screw diameter and pitch 5mm[cite: 721].

## 3.3. Used Equipments Specifications
[cite_start]**COORD3 Universal CMM machine:** Offers a bridge structure with a rotary head, allowing it to move in 5-axes[cite: 730]. [cite_start]Equipped with the RENISHAW system, Perception laser head and controlled by Touch DMIS system[cite: 731]. [cite_start]This setup enables the machine to scan the surfaces and the features of the workpiece with the stylus[cite: 732].

![CMM Setup](path/to/image.jpg)
## 3.5. Measurements Results
[cite_start]The measured points for the surface of the workpiece and the sliding jaw side of the vise with the different clamping torques were exported and then combined using MATLAB to generate the graphs[cite: 752]. [cite_start]The results showed not only deformation but also translation in z axis which can have several reasons such as the moving jaw of the vice[cite: 1084].

![MATLAB Graph](path/to/image.jpg)
[cite_start]The Heat map helps visualize and simplify the obtained results, and it clear that the z translation is happening with a constant amount for every 10 Nm for all workpieces which can be considered an interesting phenomenon as only conveying was expected[cite: 796].

## 3.6. Computer Aided solution setup
[cite_start]In the FEM simulation, A simplified geometry of the vice jaw was created and assumed as a rigid body to simplify the simulation[cite: 801]. [cite_start]The workpiece was modeled and set to be a flexible body, and the material model was added according to the aluminum alloy "AlMgSi1" as young modulus 70 GPa and poisson's ratio of 0.33[cite: 804].

![FEM Mesh](path/to/image.jpg)
## 3.7. Computer Aided solution results
[cite_start]The Parametric function of ANSYS was used to easily edit the geometry and the applied forces and generate all the needed results[cite: 815]. [cite_start]The ANSYS simulation showed similarity with the deformation value of the CMM measurements[cite: 820].

![ANSYS Results](path/to/image.jpg)
---
[cite_start]**Author:** Bishoy Romany AbdAlmasih Labib [cite: 1]
[cite_start]**Thesis:** Optimization of medical device manufacturing technology [cite: 16]
