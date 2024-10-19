# Healthcare-Data-in-Power-BI


In this case study, I'm analyzing a healthcare dataset to uncover hospital efficiency insights for a fictional consulting company, HealthStat. The focus is on exploring factors that impact patient Length of Stay (LOS) and healthcare costs, aiming to identify what contributes to variations in hospital performance.

Throughout this project, I'm leveraging DAX to create powerful measures and building insightful visualizations using Power BI. 

Some DAX measures that I used : 
Total Hospitals = 
DISTINCTCOUNT(
    hospital_discharges[facility_id]
)

% Var Average Cost per Discharge = 
VAR vAVG = [Average Cost per Discharge]
VAR vAvgALL = CALCULATE([Average Cost per Discharge],ALL())
RETURN
(vAVG-vAvgALL)/vAvgALL

% Var Average LOS Days = 
VAR vAVG = [Average LOS Days]
VAR vAvgALL = CALCULATE([Average LOS Days],ALL())
RETURN
(vAVG-vAvgALL)/vAvgALL

Snap of My PowerBI report 

![healthcarepowerbi1](https://github.com/user-attachments/assets/53292a17-19cb-4fea-a691-0d5f7becde3d)

![powerbi2](https://github.com/user-attachments/assets/f79353fe-d439-4da0-bf8e-f78ec21ef1be)

