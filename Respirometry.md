# Respirometry SOP

### Prepared by: Coral Reef and Ocean Health Research Group
### Last updated: February 5, 2025
### Pre-requisite SOP: NA
### Safety precautions: **Required PPE - <ins> none </ins>**

## Purpose: 
The purpose of this SOP is to detail the methods for setting up and using the Automated intermittent respirometry software, AutoResp™ 2.3.0. This software is owned by Loligo Systems. AutoResp™ 2.3.0 is user-friendly Windows software to be used with Loligo’s automated intermittent respirometry systems allowing users to jump-start oxygen consumption measurements in aquatic organisms. The computerized multi-channel systems with fiber optic oxygen sensing technology offer unbeaten efficiency, accuracy, and time resolution of aquatic respiration data.
  - [AutoResp™ User Manual](https://loligosystems.com/media/cxqnbvfh/autoresp-user-manual-230.pdf)
  - [Witrox User Manual](https://loligosystems.com/media/v41dxbua/quick-guide-witroxview-1_2.pdf)
  - [Netio User Guide](https://www.netio-products.com/files/download/sw/version/NETIO-4x-MANUAL-en_1-3-0.pdf)

### Materials:
1. Respirometry Laptop
2. Witrox Data Acquisition Systems (Loligo Systems, Wiltrox 4)
3. Oxygen sensors (flow-through cells)
4. Oxygen probes
5. Chamber system setup

### Background Theory:
**Intermittent Respirometry**
AutoResp™ is based on the principle of intermittent respirometry aiming at combining the best of both of the above methods
  1) closed
  2) flow-through respirometry. 

The experimental animal is placed in a sealed chamber with ports for recirculating the (closed) volume of water inside the chamber during measurements to avoid gradients (mixing) and to maintain adequate flow past oxygen probes with self-consumption of oxygen. 

A second set of ports are used to flush the water inside the respirometer chamber intermittently with water from the ambient tank (temperature bath) in which the chamber is submerged to avoid severe oxygen depletion inside the chamber. Hence the name intermittent respirometry. 

A computer actuated (flush) pump connected to the latter ports is turned on and off intermittently to flush the chamber, When the flush pump is turned off the systems operates like closed respirometry. 

When the PC controlled flush pump turns on, it pumps ambient water into the respirometer chamber thus bringing the oxygen content to the level of the surrounding ambient water. In this way, problems with accumulating metabolites and severe changes in oxygen level due to animal respiration are avoided. As with open (or flow-through) respirometry, the duration of the experiment is in principle unlimited.

However, the most important advantage is the great time resolution of this method. Oxygen consumption rates of animals can be determined for every 5-10 minutes over periods of hours or days, making automated systems extremely well suited for uncovering short and long term variations in respiration. 

In summary, AutoResp™ systems for automated oxygen consumption measurements have been developed for prolonged respirometry experiments in a controlled laboratory environment. 

To summarize, the automated measuring procedure runs in three phases: 
  1. Measuring period (M) 
  2. Flush period (F) 
  3. Wait period (W)

In the Measuring period (M) the flush pump is off, and the chamber is closed. Fish respiration rate is calculated from the decline in oxygen. During this time the recirculation pump is active to mix the water inside the respirometer and to ensure proper flow past the oxygen sensor.

The measuring period is followed by a Flush period (F) where the flush pump is active pumping water from the ambient temperature bath and into the respirometer. During this period the recirculation pump is inactive and the oxygen curve will raise to approach the level of the ambient water.

Finally, the flush pump stops and the loop ends with a short Wait period (W) before starting a new measuring period. This waiting period is necessary to account for a lag in the system response resulting in a non-linear oxygen curve. During the Wait period the recirculation pump is active.

**Dissolved Oxygen**
The oxygen capacitance coefficient ß in water is only 1/30 of that in atmospheric air, depending on barometric pressure. The concentration of oxygen in air-equilibrated water depends on water temperature and salinity. Even more importantly, the diffusion velocities of oxygen molecules are 10.000 times lower than in air. Thus oxygen is scarce and fluctuates due to environmental changes in pressure, temperature and salinity.
- [O2] = pO2 ⋅ β
- [O2] = concentration of oxygen in water (mgO2/l)
- pO2 = partial pressure of oxygen in water (kPa)
- β = capacitance coefficient of oxygen in water (mg O2/l/kPa)

Atmospheric air contains c.21% oxygen, e.g. 210 mlO2/L and in general terrestrial animals is rarely challenged by any significant changes in oxygen availability. In comparison one liter of “saturated” water in equilibrium with atmospheric air, contains only c.10 mlO2/L, and oxygen solubility will decrease with increasing water temperature and salinity and visa versa.

Thus, many aquatic organisms experience significant perturbations in oxygen levels in their natural environment, and not only due to anthropogenic effects. In environments with high biological activity, algae and plants can add high amounts of oxygen to the water during daytime photosynthesis, whereas oxygen in the water is consumed during night by the respiration of the same organisms and bacteria in some case causing severe hypoxia.

Formulas
- [O2] = PwO2 ⋅ β

Where
- PwO2 = oxygen partial pressure in water (kPa)
- ß = oxygen solubility in water (mgO2/l/kPa)

From barometric pressure (BP) and vapor pressure (pH2O) the partial pressure of oxygen in fully saturated water can be calculated as:
- pO2= (BP – pH2O) ⋅ 0.2094
- where 0.2094 is the fraction of oxygen in the atmosphere at sea level.

### Step 1: Setup
- To use AutoResp™ 2.3.0 software, the PC user must have Adminstrative status on LSCI 23122085 (Repsy Computer)
  - To obtain Workstation Admin Request, please see the following instructions. 
- Start AutoResp™ from the start menu in Windows. Make sure to right click and run the program as “Administrator”. 
  1. Right click on the AutoResp™ icon.
  2. Choose properties.
  3. Go to compatibility.
  4. Enable “Run this program as an administrator”
  5. Click OK.
  6. Now open AutoResp™ by double clicking the icon.
  7. Choose Yes, to confirm that you want to start the software as admin.
- AutoResp™ will start in the screen mode shown below. Here you can connect the different instruments that you have, and configure the input channels.
  - Data Aquistion Instrument (DAQ): Netio, Com Port: COM 3
  - Fiber Optic Instrument N°1: Witrox 4; Com Port: COM4
  - Fiber Optic Instrument N°2: Witrox 4; Com Port: COM7
- Selection of units of measure.
  - In AutoResp™ users can freely choose between the oxygen units % air saturation, kPa (partial pressure of oxygen) and mgO2/L (oxygen concentration), but this requires a user input for barometric pressure and salinity.
    - Be sure to look up barometric pressure for your location and record.
  - Temperature is also required, but can be acquired automatically if connecting a temperature instrument to each Witrox. Because there is only 1 temperature probe per Witrox, the user must be careful that temperatures remain stable across all chambers within the Witrox cluster.

![Picture1](https://github.com/user-attachments/assets/c3395e87-fa9b-464b-ab51-b5cbc2abc7e5)

### Step 2: Oxygen Calibration
- Oxygen Calibration in AutoResp™
  1.	The digital output from the oxygen instrument must be calibrated in the AutoResp™ software to show correct oxygen values. 
  2.	Make sure all oxygen probes are attached to appropriate Witrox DAQ.
  3.	Measure at 0% air saturation, and press LOCK LO. Since fiber optic oxygen sensors are sensitive to temperature, it is also necessary to enter this value. 
    i.	This is often done by bubbling with nitrogen gas or use a sodium sulphite solution to remove all oxygen from the setting the measured (LO) value to 0%. 
  4.	Measure at 100% air saturation, and press LOCK HI. Since fiber optic oxygen sensors are sensitive to temperature, it is also necessary to enter this value. 
    i.	This is often done by equilibrating a stirred water sample with atmospheric air to reach 100% air saturation. Use an air pump to bubble the water sample and allow enough time for full equilibration. Then place your oxygen sensor in the sample and wait for the sensor signal to stabilize. Then follow the operating instructions for the meter to set the measured (HI) value to 100%. 
  5.	Choose Online (Ambient) as temperature input channel. It is very important to temperature compensate the fiber optic oxygen values, since the oxygen values are very temperature dependent. 
  6.	Repeat this step for every oxygen channel.
  7.	The calibration and configuration is continuously saved to a binary file (AutoResp.conf).
  - Calibration file will be saved in two of three places
    i.	Teams
    ii. GitHub
    iii.	Desktop

### Step 3: Starting an Experiment
- Following oxygen calibration, choose Experiment  Start to start a respirometry experiment.
- Before the experiment starts a number of parameters must be given in order for AutoResp™ to calculate oxygen consumption rate etc. 
  - First enter the chamber volume and choose the correct unit.
  - Enter the volume of tubes in the recirculating loop only and choose the correct unit of measure. In swim tunnels this tube volume should be set to zero (0).
  - Enter the wet weight of the animal(s) and choose the unit of measure.
  - The wet weight of the coral.
  - Then enter the density of the animal(s) for the software to calculate the respirometric volume.
  - Density of corals: Density = Mass / volume.
  - The respirometric volume is calculated as:
    - Resp. volume [L] = chamber volume + tube volume - volume of organism(s)
  - The ratio field indicates the ratio between the Resp. volume and the wet weight volume. As rules of thumb, this ratio should be 10-20 for measurements in resting animals (like corals) for reliable M02 measurements.
    - If experimental temperatures are high, the ratio can be higher without compromising the quality of MO2 data.

<img width="352" alt="Picture1" src="https://github.com/user-attachments/assets/64dfe4bf-090e-4a01-927a-b899a0f5862b" />

- When complete, please OK.
- Now a file dialog pops up, where the user is asked a file path for the (calculated) data file and raw data file. The raw data file will get the same name as the data file but with “_raw” as an extension to the file name.
  - All data will be saved in two of three places
    i.	Teams
    ii. Github
    iii.	Desktop

<img width="361" alt="Picture1" src="https://github.com/user-attachments/assets/829e0d32-ce7b-465f-bd4c-4566188d6708" />

- Now an experiment is started, but in a continuous flush mode so that no oxygen consumption measurements will take place until the user sets the operation to either “Close” (closed respirometry) or Intermittent (intermittent respirometry).
- Move the mouse over the relay indicator diodes in the upper right corner. A Help text will pop up and help the user which relay is used as recirc, flush, ambient control etc.
- The upper screen shows the oxygen values for the chambers. Right clicking on the graph will show a submenu. It is here possible to hide/show chamber graphs, pause graphs, scale axes etc.
_Note: AutoResp™ will continue collecting data even though graphs are set on pause (Show cursor). While set on pause the x-scrollbar appears and it is possible to go back to the start time of the experiment using the scrollbar._
- The lower graph panel shows the data and graphs for calculated values.
- The Data tab will show all current values. Some fields are gray, depending on the configuration mode. So in the current example case, chamber 1 and 2 are shown and the ambient temperature only.
- Because the ambient temperature was activated, an ambient Temp tab is also accessible, showing ambient water temperature in real time or average values over time (right click). Depending on the configuration, different tabs may appear, such as ambient oxygen, Uspeed (swimming speed) etc.
- In the upper right corner, the kind of experiment currently running can be chosen.
  - Flush – This means that the flush is always on. The object will get new sump-water constantly, but this also means that no MO2 values are calculated.
  - Close – This means the chamber is closed, and every time a measure period is finished a MO2 is calculated. After the measure period is finished a new measure period will begin immediately. 
If choosing this mode of operation, take care not to leave the set up to avoid severe oxygen depletion inside the chamber due to animal respiration.
  - Intermittent – This means the experiment runs in a loop (flush, wait and measure). During each flush period, the flush pump is turned on to flush chambers with ambient water. The wait periods allow time for steady state before measurements start during the measure period. In Intermittent mode, the skip phase button allow users to jump between these three modes (flush, wait measure) immediately and on-the-fly for special applications or situations, e.g. to start flushing the chamber immediately after reaching Ucrit during a swim trial. 
  LOOP 
  F1->W1->M1->F2->W2->M2 etc. 
**Adjusting Experimental Settings**
- SettingsGeneral to set the settings for the experiment.
- In the General settings it is possible to change oxygen units, water salinity or barometric pressure during experiments. It is also possible to change flush, wait and measure times.
  - Flush times should be set to allow complete renewal of water inside each chamber. This will restore oxygen values to ambient between each measurement. As a rule of thumb, cylindrical chambers should be flushed with a volume five times the chamber volume for 99% wash-out, but this depends on chamber dimensions.
  - The measurement times should allow enough data for a reliable determination of the slope of the oxygen curve to be estimated. The slope is determined from a linear regression, and the regression coefficient r^2 express the statistical validity of the calculated slope, e.g. r^2 >0.95 indicates a sound linear relationship (oxygen vs. time), and thus a reliable MO2 value.
  - Notice that the recirculating pump can be set to constant activity. This will double the flow during flush periods potentially affecting animal behavior/locomotion, but will provide better oxygen readings if the oxygen probe is placed outside the chamber in a recirculating loop.
- The MO2 analysis buttons are gray during measurements, but can be used during post analysis when loading saved raw data files form past experiments.
- Press OK to close the general settings.
- Now run an experiment for min/hours/days depending on application. Adjust your settings during measurements if needed. Any changes will be written in the raw and data file.

<img width="349" alt="Picture1" src="https://github.com/user-attachments/assets/5f674c60-9404-45a2-b028-ddcd75858480" />

_Your graph should look like this. This is a graph for one chamber only._
- To end the experiment, click Experiment -> Stop.
- Now press File->Load to analyze saved data. The file loading might take a while.
- When the file is loaded, a new tab labeled Stats are now available for the user. Use this tab for calculations and statistics.

<img width="356" alt="Picture1" src="https://github.com/user-attachments/assets/682549af-ea2a-4de8-85e3-2600ad40ddb7" />

**Data Analysis**
- The analysis settings are available in Settings General.
- Choose SMR estimation method and choose a minimum average oxygen level for estimating standard metabolic rate (SMR) to exclude any hypoxic values. For hypoxia experiments, the critical point for metabolic homeostasis (Pcrit) can be calculated automatically. Click the button to set the number of low oxygen values that should be part of the oxy-conforme curve when the animal is no longer able to regulate respiration rate independently of ambient water oxygen.

<img width="410" alt="Picture1" src="https://github.com/user-attachments/assets/37277635-0896-4569-913c-f0d5dcc7fc8f" />

### Quality Assurance and Control Methods
Proper protocols and training must be implemented to ensure the quality of data generated in the laboratory. Quality control measures are outlined in each protocol to ensure data generated are of accurate quality. Researchers must ensure that all equipment is accurately calibrated, inspected, and maintained according to the manufacturer’s instructions. Data must be entered in Excel spreadsheets by one individual and QA-QC checked by a different individual.  
 
_Data Review_

All laboratory data will be reviewed for completeness and transfer errors. Data will be reviewed by a second individual after entry into Excel spreadsheets by comparing the entered, electronic data to the original records (e.g., hand-written datasheets or laboratory notebooks).  Data will be summarized as descriptive statistics and in tabular and graphical form to allow visual inspection and verification, and comparison to expected or target values.   
 
_Data Verification_

Data will be checked for compliance with the procedures outlined in the SOPs and OPs.  Any deviations from those procedures and the impact on the quality of the data will be assessed and discussed with Task Members. Any laboratory data outliers will be flagged. 
 
_Data Validation_

Once the data has been reviewed and verified, it will be assessed to determine the overall acceptability of the objectives of the project.  Blank samples, such as with water quality testing, will be used to determine any biases or instrument calibration issues during the sample collection and analysis processes.  Control samples will be used to determine the condition of the experimental test specimens in the absence of experimental treatments or exposures.  Any errors in datasets detected will be discussed with lab members and project leads to determine the impact on the data and its use for the project.  If there are any limitations to the data, they will be disclosed as part of the published literature. 

_**Procedure Specific QA/QC Methods:**_

_Sensor calibrations_

Oxygen sensor calibrations for intermittent flow respirometry are conducted before each experimental trial using two known standard solutions (i.e., air saturation for high value (100%) and sodium sulfite for low value (0%). An air pump is used to allow for full air-saturated water to calibrate all oxygen sensors. Then sodium sulfite (or yeast – depending on availability) is mixed into distilled water to remove all oxygen from the sample for 0% calibration. Oxygen sensors are placed into calibrations until the sensor signal stabilizes. The oxygen meters convert sensor values to percent (%) oxygen saturation. The signal value of each probe is recorded to track sensor stability. Sensors are then cleaned with ethanol and stored in the dark to maintain probe quality and conditions- following the recommendations of probe manufacturers.

_Data collection_

Oxygen (% saturation) readings are collected every second throughout the intermittent flow experiment. Intermittent meaning each chamber runs in a loop (flush, wait and measure) cycle. During each flush period, the flush pump is turned on to flush chambers with ambient water. The wait periods allow time for a steady state before measurements start during the measure period. Times between each period (flush, wait, and measure) are dependent on the size for the organisms and volume of water. These times are recorded for each experiment are determined based on oxygen consumption rates of organisms from preliminary trials to ensure percent saturation is above 80% (Svendsen et al., 2016). Pre-determined times between measurements allows for enough data for a reliable determination of the slope of the oxygen curve to be estimated. The slope is determined from a linear regression, and the regression coefficient r^2 express the statistical validity of the calculated slope, e.g., r^2 >0.95 indicates a sound linear relationship (oxygen vs. time), and thus a reliable oxygen consumption value (MO2) value.



















