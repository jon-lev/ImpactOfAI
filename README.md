# ImpactOfAI

## PDTB Treebank 2.0 Dataset
- PDTB Dataset requires a LDC license, so the data cannot be distributed by us.
- Dataset can be obtained here: https://catalog.ldc.upenn.edu/LDC2008T05

## BERT Parser (https://github.com/najoungkim/pdtb3)
- Requires the PDTB dataset to be in .csv format
  - Can be obtained here: https://github.com/cgpotts/pdtb2
### Steps
1. Setup data paths in preProcessing function in BERTParse.ipynb
2. Run preProcess function
3. Change data paths and settings in test_run.sh before running
4. Run powerUsage.ipynb once iterations begin
5. Manually running powerUsage.ipynb cell once iterations end 
6. Use csvCalculation.ipynb to examine results

## Non-bert (Java) Parser (https://github.com/WING-NUS/pdtb-parser)
- Trained and tested on PDTB data

### Steps
1. Setup data paths in config.properties before preprocessing and running
2. Follow the steps on the parser's repository to determine which .jars to run
3. Use rapl_power_meter and nvidia-smi commands while running to determine power usage
4. Can use csvCalculation.ipynb to examine results of .csv outputs of rapl_power_meter and nvidia-smi
