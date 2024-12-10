# 3D Scanning and Surface Area Measurements

## Prepared by: Coral Reef and Ocean Health Research Group; Adapted from Dr. Davies Lab at Boston University
## Last updated: December 9, 2024
## Pre-requisite SOP: NA
## Saftey precautions: **Required PPE - <ins> enclosed shoes </ins>**

## Purpose: 
The surface area of the corals will be measured using a 3D scanner (EinScan-SE). More recent work has shown that 3D-scanned images 
of the coral provides a more accurate surface area measurement, which is needed to standardize physiological measurements.

### Materials:
1. Scanner manual - can be found [here](https://support.einscan.com/en/support/solutions/60000333808manual/?scan_model=einscan-se&download_option=manual)
2. Calibration object (Ex. a die with a known area)

3. Manilla file folder
4. Pedestal for coral branch
5. Dry coral skeletons
6. Hard drive
7. White background

### Equipemnt and Software:
1. Einscan-SE 3D Scanner V2
([link here](https://www.matterhackers.com/store/l/einscan-se-desktop-3d-scanner-v2/sk/M21W1D74?rcode=PMAX_3DSCANNERS&gad_source=1&gclid=Cj0KCQiAx9q6BhCDARIsACwUxu7pOD51OZK9U7pb7UIQv4JnsGah-zn-YAVN4FoepX1He3ohGdny0QIaApx_EALw_wcB))
2. Einscan-S software
3. Hard drive

### Notes: Glue broken corals together with coral glue if necessary.

### **<ins>Step 1 - Scanner setup:</ins>**
1.	Ensure that all the power and computer connection cables are plugged in (scanner power, cable from scanner to computer, and cable from scanner base to scanner camera). 
2.	Turn the scanner on by touching the power button (it’s touch-sensitive) 
3.	Make sure the scanner is completely in the dark (under a black box). 
4.	Make sure the background of the scanning area is completely white.

### **<ins>Step 2 - Running the software:</ins>**
1. Open the Einscan-S software. If you do not have this installed, it can be downloaded [here](https://www.einscan.com/support/download/software/?scan_model=einscan-se)
2. Click on Einscan-SE (left logo)
3. The scanner in the lab should already be calibrated, but if you want to redo the calibration just to make sure (or if it’s been a while since it’s been used):
  The calibration object is in the drawer to the left of the scanner/computer (it looks like the logo on the program's screen).
  - Note: If the scanner has been relocated, then DEFINITELY RECALIBRATE.
  - Follow directions on the screen
  - If your scan is coming out yellow, then you need to redo calibration and white balance. There is something wrong with the white balance and that is why the background of the scanning area needs to be completely white.
4. Click on Fixed Scan.
5. Click on New Project (if you open the program before turning on the scanner you may not be able to click on new project, quit the program and re-open).
6. Select Texture scan
  - It will ask you if you want to restart the white balance.
  - It is recommended re-doing white balance whenever you open the program for the first scan, for subsequent scans in the same day, with the same lighting you do not have to re-do it.
  - To do the white balance hold up a white sheet of paper in between the scanner base and the scanner camera (the program also shows you a diagram).
7.	Place your coral on the scanner base. 
8.	You should then check the brightness of the scan in the “Scan Settings” tab, select the shade from the slider such that the object you want to scan (i.e., the coral) is barely highlighted in red in the camera preview. There should be very little red on the object and none on the background.
9.	TURN ON THE HDR OPTION with the slider button after changing the brightness. This is important for scanning corals otherwise you get unusable scans.
  - Coral should be slightly red on the screen with a white background.

| ![Picture1](https://github.com/user-attachments/assets/2e3f4e54-c241-4950-9d02-89396ae8c8ad) | ![Picture2](https://github.com/user-attachments/assets/5376f30e-680c-4f1b-9247-89683a814d86) | ![Picture3](https://github.com/user-attachments/assets/036c0d58-f24c-4d03-a152-26f36ff50513) |
| :---: | :---: | :---: |
| Too dark| Perfect brightness: Specs of red on the coral | Too bright | 

10. Select “with turntable”
  - The default number of turntable steps is 12. I find this to be sufficient. 
11.	Double check that HDR is on and make sure your coral is balanced and will not fall. 
12.	Click Start Scan
  - You will see the scans start appearing on the screen. It will turn the object and scan 12 times (or however many steps you specified). Once the set of scans is done you will have the option to edit the scan. For instance, you can select certain parts and delete them. Do this now to delete the stand from the scan as not doing so will not allow the scans to align.
  - If things look good, then click on the green check mark. 
13.	Rotate your object slightly on the turntable (but keep it in the same location) and start another set of scans. Repeat this twice for a total of three scan sessions per coral. 
14.	DO NOT globally optimize between scans. Optimizing increases the number of points and can overload the machine and invalidate the scans. 
  - If you find the scan looking abnormal, you may need to check if the scan will optimize by clicking the “Global Optimization” button, but don’t finalize the optimization. If the scans are not optimizing and look abnormal, recalibrate the machine.

### **<ins>Step 3 - Editing the final scan:</ins>**
15. You may have had to place your coral on a pedestal to scan it (especially if it's something that couldn’t stand on its own like a branch). 
16.	You can now delete the scans of the pedestal and any extra parts that are not useful. To do so: 
  - You can select the areas in the scan by holding down the shift button and making a circle with your mouse:

<img width="111" alt="Picture4" src="https://github.com/user-attachments/assets/977cf6e3-02d3-4d00-96bc-5c760895bba6"> <img width="108" alt="Picture5" src="https://github.com/user-attachments/assets/3559d7d1-13dc-464c-baed-38400f1c7ea3">

  - This will select a region of the scan.
  - Then you can delete the region by clicking on the delete button in the edit tools area.\

<img width="110" alt="Picture6" src="https://github.com/user-attachments/assets/0d9117ef-5a3b-4f92-b3fe-01917b74cc8a">

### **<ins>Step 4 - Saving and Exporting Final Scan:</ins>**
1. Once you’re satisfied with your scan, click on Global Optimization on the right-hand side of the screen and then click the check mark
2.	Click on Mesh in the right-hand side of the screen
3.	Select watertight model 
4.	Select high detail (or the level of detail you require, for most corals we’ll want high). 
5.	Click apply (decide whether you want to smooth/sharpen, in most cases you won’t) 
6.	Then click Save your scan. 
7.	When saving also select the “.ply” option 
8.	To start new scan go back to “scan” and click the project icon, work, new work, and start new scan. 

### **<ins>Step 5 - Calculating the Surface Area Using Meshlab:</ins>**
1. Open the “.ply” (or .stl file also work) using MeshLab. 
2.	Use the appropriate method for selected the surfaces that you want to measure the area of: 
  - If your coral nubs were essentially all live tissue: then then easiest route may be to calculate the surface area of the entire scan and then subtract the surface area of any spots that were not coral (e.g., the bottom of the nubbin/branch) 

<img width="198" alt="Picture7" src="https://github.com/user-attachments/assets/a1113b79-830e-4c0e-bf27-8d4469006c33">

  - Select the entire scan surface using the “Selected connected components in a region” button and dragging across the whole scan to select everything. (Selected areas appear pink) 
    - Calculate surface area of selection. Menu path: Filters -> Quality measures and computers -> Compute Area/perimeter of selection
    - The computed area will appear in the dialog box in the lower right-hand side. **The units are in square millimeters**.
<img width="198" alt="Picture8" src="https://github.com/user-attachments/assets/496ef0ed-af20-4a00-b7a3-db65ce6f8c1e">
    - Deselect everything by pressing shift-D when the selection tool is engaged.
    - Click on the Selected connected components in a region button again to deactivate the tool.
    - Then use the z-painting tool to select the areas that you need to subtract. Menu path: Edit->z-painting tool. Then click on the red paintbrush icon. Increase hardness to 100 and adjust the size of the bubble as needed.
<img width="198" alt="Picture9" src="https://github.com/user-attachments/assets/0e460ae7-26f5-4f6e-8c69-1f43bf975352">
    - You can then toggle between using the paintbrush and rotating the scan by pressing the escape button.
    - Paint the areas that you want to calculate the area for:
<img width="198" alt="Picture10" src="https://github.com/user-attachments/assets/f93f1d10-3005-43a5-af2e-da9d5d7c5581">
    - Once you have selected all the areas you want then compute the area/perimeter of selection again (step ii above).
    - Then subtract the numbers as needed to get your final surface areaa
<img width="110" alt="Picture11" src="https://github.com/user-attachments/assets/763d6911-7dff-406f-a364-c33d43486e96">

  - If your nubs are patchy live/dead areas: Proceed directly to just using the z-painting tool to select the areas of the nub that were live, and you want surface area for. Make sure to rotate the scan and ensure that the polyp valleys are well selected. E.g., avoid this:
3. Rotate and paint until everything is well selected:

<img width="110" alt="Picture12" src="https://github.com/user-attachments/assets/4a529a85-5735-4902-8978-2bc24a7bb3e6">

4. Then compute the area of selection (see above)

### **<ins> Notes:**</ins>
  - For larger colonies turn down the brightness to help with detail (intricate branching) and increase number of turntable steps to the maximum and scan coral 5+ times depending on coral.
  - Ensure the color of your scan is correct before saving. A yellow scan means the white balance, or the background is incorrect.
  - *Please move all saved scans to hard drive after finishing a session* The computer does not have enough power or storage to hold and access a lot of scans.

### **<ins> Quality Assurance and Control:</ins>**
_Proper Training_

Proper protocols and training must be implemented to ensure the quality of data generated in the laboratory. Researchers must ensure that all equipment is accurately calibrated, inspected, and maintained according to the manufacturer’s instructions.

_Data Review_

All laboratory data will be reviewed for completeness and transfer errors. Data will be reviewed by a second individual after entry into Excel spreadsheets by comparing the entered, electronic data to the original records (e.g., hand-written datasheets or laboratory notebooks).  Data will be summarized as descriptive statistics and in tabular and graphical form to allow visual inspection and verification, and comparison to expected or target values. 
 
_Data Verification_

Data will be checked for compliance with the procedures outlined in the SOPs.  Any deviations from those procedures and the impact on the quality of the data will be assessed and discussed with Task Members. Any laboratory data outliers will be flagged.
 
_Data Validation_

Once the data has been reviewed and verified, it will be assessed to determine the overall acceptability of the objectives of the project.  Blank samples, such as water quality testing, will be used to determine any biases or instrument calibration issues during the sample collection and analysis processes.  Control samples will be used to determine the condition of the experimental test specimens in the absence of experimental treatments or exposures.  Any errors in datasets detected will be discussed with lab members and project leads to determine the impact on the data and its use for the project.  If there are any limitations to the data, they will be disclosed as part of the published literature.

_Procedure Specific QA/QC Methods_

_3D Scanner_

Three-dimensional scanner is calibrated when necessary, according to calibration procedures described in the instrument manuals. To prevent errors in the processing of the scanned data, only technicians trained on the 3D scanner and software will be permitted to use the equipment.




    








 











