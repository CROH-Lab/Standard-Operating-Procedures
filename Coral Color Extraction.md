# Protocol for extracting color from coral photographs

## Prepared by: Coral Reef and Ocean Health Research Group; Adapted from Putnam Lab
## Last updated: December 9, 2024
## Pre-requisite SOP: NA
## Safety precautions: **Required PPE - <ins> enclosed shoes </ins>**

### Purpose: 
Coral color is a common measurement used to indicate coral health or coral stress (Chow, Tsang, Lam, & Ang, 2016), with a negative correlation between the intensity of the red (RGB) channel and the density of chlorophyll (Winters et al., 2009).  
The maximum of the red channel spectrum (255) represents white, and the minimum (0) represents true red, with this color range being used as a rough proxy to quantify symbiont cell density. 
Coral color was analyzed using photographs taken at the same angle and distance using a digital camera (Canon EOS2000D) and a controlled typology-based setup. 
Camera parameters including mode (M for manual), aperture (f10), ISO (200), shutter speed (1/30), and white balance (auto) were manually set and remained consistent across most images. 
A commercial underwater color reference card (DGK Color Tools WDKK Waterproof Color Chart) was placed behind the coral fragments. 
Color values must be extracted from these images using Photoshop in order to assess color trends.

----

### Content:

[Materials](#Materials)

[Protocol](#Protocol)

[Quality Assurance and Control Methods](#QA/QC)

----

<a name = "Materials"></a>
### <ins>Materials</ins>
1. Adobe Bridge (for file organization)
2. Adobe Photoshop (color extraction)
3. .RAW images
4. Microsoft Excel

----

<a name = "Protocol"></a>
### <ins>Protocol</ins>

1.	Organize coral files in Adobe Bridge according to experimental parameters (do this PRIOR to any analysis). 
  - .RAW photos should be clear, and show the coral fragment, the color reference card, and the sample name.
  - Have available folders:
    - RAW Images (for batch editing Raw files)
    - Area Selected (to save areas of coral used in color indexing)
    - Color Tables (for saving swatch groups for each image)

2. Select the best photo for each coral as defined by XXXX

3. ***For lab-setting/controlled images*** **Prepare images** by Batch editing files in Adobe RAW (Included in Bridge/Photoshop)
- Copy all images into the RAW folder to batch edit.
- Mass-select images to be analyzed (called batch editing) by clicking Ctrl+A or Command+A and click the camera RAW icon to open in Adobe RAW
- Mass-select images in Camera Raw again using Ctrl+A or Command+A so edit all images at once.
- Click setting link on bottom of window and input correct camera settings (Camera raw prefernences (only needs to be done once per profile): workflow: Preset = Custom; Space = Adobe RBG (1998); Depth = 8 bit

![Picture1](https://github.com/user-attachments/assets/f1d7ea8f-247d-4251-a082-02e258ddf5a9)

- In optics: Check boxes for ‘remove chromatic aberration’ and ‘use profile corrections’ (make sure camera used in photos is selected)

![Picture1](https://github.com/user-attachments/assets/eec062b7-6207-45ef-8fc0-d9146fccfc9b)

- In Details: Adjust Sharpness to 25

![Picture1](https://github.com/user-attachments/assets/e85ab615-ae36-48d3-9bca-0d70f748f111)

- In color: White Balance image by selecting the dropper tool and clicking on a non-distorted, clear portion of the white color swatch on the calibration card. Adjust brightness as needed (may need +1 brightness) if white balance is off. Please try to not adjust the brightness.
- Click Done to edit all images.

![Picture1](https://github.com/user-attachments/assets/b2e240b5-44ed-41a3-bfa4-604a4d443eea)

Select image(s) to open in photoshop.

4. Correct image colors (for field/uncontrolled images): white, grey, and black balance using the curves adjustment. 
- DO NOT batch edit. Open an Image in Photoshop as a smart object using the same Camera Raw setting as above.      

<img width="468" height="276" alt="Picture1" src="https://github.com/user-attachments/assets/887af747-2575-43da-bb30-8a73e48f1b54" />

Press open at the bottom left to enter photoshop and make sure the image is 6bits channel

<img width="468" height="273" alt="Picture1" src="https://github.com/user-attachments/assets/6faae73e-0e5a-4075-a849-345109a6db9a" />

  - Open a new curve layer by selecting adjustments -> curves

![Picture1](https://github.com/user-attachments/assets/7a9c8ad2-5d24-4745-9448-d167052341ee)

<img width="468" height="234" alt="Picture1" src="https://github.com/user-attachments/assets/e63e6c95-17e2-4e55-bd85-e1d8ac4b87ef" />

  - Find the dropper icons on the bottom of the chart

<img width="468" height="234" alt="Picture1" src="https://github.com/user-attachments/assets/cbbc788e-8119-4b15-9092-e9d109b541e3" />

  - Select each dropper and click the corresponding correction swatch on the color correction card in the image. The black, grey, and white dropper each have their own icon.
    - Choose which grey (neutral) swatch works the best, and use the same swatch for consistency press OK

5.	Color Extracting
- Open batch-edited coral image(s) in Photoshop (or take color-curve corrected image that is already open).
- Select the coral using quick select. 

|![seelct](https://github.com/user-attachments/assets/e21bd888-eb93-4249-a661-bea6d6845b8c)|![coral select](https://github.com/user-attachments/assets/50564e2d-7dc1-48eb-ace1-eecd89c11a60)|![only coral](https://github.com/user-attachments/assets/e098f968-3896-4c51-9126-af204978b482)|
|:-:|:-:|:-:|

<img width="468" height="250" alt="new coral select" src="https://github.com/user-attachments/assets/94046433-7b40-46e9-8bfa-8505c0821c1e" />

- Command+(or Ctrl+)C, Command(or Ctrl+)V to put the coral area only on a different layer.

<img width="468" height="305" alt="Picture1" src="https://github.com/user-attachments/assets/60ac7582-cb41-48d9-acfa-f0d4c628494f" />

- Create a mask of the image by clicking this icon on bottom right of window. Hide the original (background)image.
  - On the bottom right of the screen deselect the ‘background’ layer so only the color curve and/or layer 1 are highlighted.

![Picture1](https://github.com/user-attachments/assets/78788fcb-558b-41d5-89f5-e87b0cf60e56)

- *Select color area*: Select mask layer and select eraser tool. Adjust tool size on left side of top toolbar and increase hardness to 100%. Paint over areas on coral to be excluded.

|![Picture1](https://github.com/user-attachments/assets/480f3c00-9f9f-4ed7-b3ba-0c882153338a)|![Picture1](https://github.com/user-attachments/assets/c4b1af87-7fd8-45cd-a536-012befa4bf15)|
|:-:|:-:|

  - Make sure the visible area excludes shadows, bubbles, calcifying tips, edges, and anything that is NOT an illuminated, clear image of coral connective tissue.

<img width="468" height="273" alt="Picture1" src="https://github.com/user-attachments/assets/0d587467-a377-4c00-87fd-c384a14fc6ff" />

  - When done, save file (Ctrl+Shift+S or Command+Shift+S) in the Area Select folder as (filename(AS)).psd. This saves the specific area to be indexed.
    - Note: changing the area of the selected coral will change most, if not all, of the swatch values. Be sure the area is adequate before color indexing.

6.	**Index the Color** by going to Image -> Mode -> Indexed Color. Merge all visible layers, which will discard the background layer. Set the Indexed Color settings to Local (selective), 11 colors (to get the top 10 colors and ignore the grey/white squares), forced: None. 

|![Picture1](https://github.com/user-attachments/assets/0b908b1d-c776-4e6a-a5ab-16309720c5b1)|![Picture1](https://github.com/user-attachments/assets/bd3c53f5-3031-400a-9e02-2ebbb5d28f25)|
|:-:|:-:|

7.	**Create the color table** in Image -> Mode -> Color Table. Save the 10 most frequent colors from each area to swatches and save as color table (filename(CT)) with .act extension. This saves the swatches.

<img width="134" height="59" alt="Picture1" src="https://github.com/user-attachments/assets/8d95d7ee-3511-4a76-848e-3a1e66cd1eec" />

<img width="468" height="198" alt="Picture1" src="https://github.com/user-attachments/assets/8a8e6c49-a90b-4570-9c06-0ad5a3f6d56f" />

|<img width="146" height="184" alt="Picture1" src="https://github.com/user-attachments/assets/c3b20c0d-0fd9-4806-adfb-bf5b955bdada" />|<img width="274" height="164" alt="Picture1" src="https://github.com/user-attachments/assets/c5aadee5-1dbd-456f-aa9b-ce713a8922e3" />|
|:-:|:-:|

![Picture1](https://github.com/user-attachments/assets/8612985c-1173-4c28-8264-6c0700a12955)

8.	Record the **RGB**, **CMYK**, and **HSB** values from each swatch (the top 10 from the color table) from each coral fragment on a hard copy paper datasheet and in a corresponding Excel datasheet. The swatches are saved in the same order and opening the .act file in photoshop will allow you to go back to them later by clicking on the square in the color tab.

|<img width="187" height="192" alt="Picture1" src="https://github.com/user-attachments/assets/df7e452b-9c9f-4ade-8ba5-0e820d785ba8" />|<img width="219" height="251" alt="Picture1" src="https://github.com/user-attachments/assets/2b0aad98-7d1e-481f-b851-70218b2b059d" />|![Picture1](https://github.com/user-attachments/assets/89d39c1f-6a22-4414-bdc5-ecf69b07955e)|
|:-:|:-:|:-:|

  - $${\color{red} WARNING!! \space}$$ Do not click on any colors external of the color table while the color table is open, it may override swatch values!!

9.	Close Color Table and image that is being worked on. **DO NOT SAVE CHANGES WHEN CLOSING THE IMAGE!!** The indexed area of the coral should NOT be saved, only the Area Selected. This will allow the re-indexing of the coral without having to save an additional file.

---

<a name = "QA/QC"></a>
### <ins> Quality Assurance and Control</ins>
_Proper Training_

Proper protocols and training must be implemented to ensure the quality of data generated in the laboratory. Researchers must ensure that all equipment is accurately calibrated, inspected, and maintained according to the manufacturer’s instructions.

_Data Review_

All laboratory data will be reviewed for completeness and transfer errors. Data will be reviewed by a second individual after entry into Excel spreadsheets by comparing the entered, electronic data to the original records (e.g., hand-written datasheets or laboratory notebooks).  Data will be summarized as descriptive statistics and in tabular and graphical form to allow visual inspection and verification, and comparison to expected or target values. 
 
_Data Verification_

Data will be checked for compliance with the procedures outlined in the SOPs.  Any deviations from those procedures and the impact on the quality of the data will be assessed and discussed with Task Members. Any laboratory data outliers will be flagged.
 
_Data Validation_

Once the data has been reviewed and verified, it will be assessed to determine the overall acceptability of the objectives of the project.  Blank samples, such as water quality testing, will be used to determine any biases or instrument calibration issues during the sample collection and analysis processes.  Control samples will be used to determine the condition of the experimental test specimens in the absence of experimental treatments or exposures.  Any errors in datasets detected will be discussed with lab members and project leads to determine the impact on the data and its use for the project.  If there are any limitations to the data, they will be disclosed as part of the published literature.
