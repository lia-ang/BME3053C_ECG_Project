# BME3053C_ECG_Project
Final project for BME3053C S2025

ECGTeam_data.zip Creation and Upload Steps:
1. Created a clean folder for storing relevant metadata: 
        
        mkdir -p ecg-arrhythmia && cd ecg-arrhythmia
2. Downloaded top-level metadata files from the PhysioNet ECG Arrhythmia dataset: 

        wget https://physionet.org/files/ecg-arrhythmia/1.0.0/ConditionNames_SNOMED-CT.csv
        wget https://physionet.org/files/ecg-arrhythmia/1.0.0/LICENSE.txt
        wget https://physionet.org/files/ecg-arrhythmia/1.0.0/RECORDS
        wget https://physionet.org/files/ecg-arrhythmia/1.0.0/SHA256SUMS.txt
        wget https://physionet.org/files/ecg-arrhythmia/1.0.0/WFDBRecords
3. Zipped the folder into ECGTeam_data.zip:

        cd ..
        zip -r ECGTeam_data.zip ecg-arrhythmia
4. Added and committed the zip file to the repository: 
        
        git add ECGTeam_data.zip
        git commit -m "Add ECG arrhythmia metadata files (zipped)"
        git push

ECGTeam_data/ecg-arrhythmia Folder Creation:
1. Created new folder for storing unziped files
2. unzip ECGTeam_data.zip

        unzip ECGTeam_data.zip -d /workspaces/BME3053C_ECG_Project/ECGTeam_Data/ecg-arrhythmia

Runing the Code:
1. Make a Codespace on Main
2. Install libraries

        pip install -r requirements.txt
3. Run cells
