# Heart + Intersections
This repository is the code which accompanies the paper "The Hearts Response to Intersections".

## Data
Data used was from the [HRI Driver Behaviour Dataset (HDBD)](https://usa.honda-ri.com/hdbd). To replicate the results of this experiement, please download the files from the `HDBD_realworld_video_task/SyncedFileswGazeAnnotation/CompleteParticipants/*` and move them to the path `data/Participant_Data/*` in the parent directory.

`data/Video_Data/Video_*/Video*.csv` contain manually labelled datapoints collected from watching the HDBD videos. 

## 1) Separate Participant Data by Video.ipynb
   - **Objective:** The notebook is designed to separate and organize participant data based on each video presented to them during the experiment.
   - **Process:**
     - The notebook reads a master data file containing all participant data.
     - It then filters the data based on specific video timestamps, which correspond to different driving scenarios.
     - The filtered data is saved into separate files for each scenario, allowing for easier analysis and experimentation later.
   - **Outcome:** Separate data files for each driving scenario, which will be used in subsequent analysis.

## 2) Removing Data Outliers.ipynb
   - **Objective:** This notebook aims to clean the dataset by identifying and removing outliers. Outliers can skew the results and lead to incorrect conclusions.
   - **Process:**
     - Participant data where the measured HR goes below 10 beats per minute, are flagged and removed as outliers
   - **Outcome:** A cleaned dataset, free of extreme outliers, which is more reliable for analysis and experimentation.

## 3) Experimentation.ipynb
   - **Objective:** This notebook conducts experiments on the processed data to explore relationships between physiological signals (like heart rate) and driving behaviors, particularly around intersections.
   - **Process:**
     - More information on the methodology taken may be found in the paper "The Hearts Response to Intersections" *TODO: Add Link
   - **Outcome:** Insights into the relationship between driving conditions (like intersections) and physiological responses (e.g., elevated heart rate or spikes in heart rate).


For any inquiries, please dont hesitate to reach out!
