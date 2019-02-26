# P-Code-Dataset

This dataset is a dump of P-Code instructions originated from malicious and benign VBA macro documents. We used a modified version of the P-Code dissassembler from Bontchev (https://github.com/bontchev/pcodedmp) where only the P-Code instructions were extracted.  

<!--Note that this is a pre-publication release. This repository as well as the paper and data are subject to change.-->

# Data

The data can be download in three (3) different ways.  
1. PCode_Instructions.csv 
2. PCode_Instructions_Duplicates.csv
3. PCode_Datasets.zip (Contains 1 & 2)

* ```PCode_Instructions.csv``` has 4 181 unique P-Code instructions. With columns such as ID, PCode, Type, and Malware.
* ```PCode_Instructions_Duplicates.csv``` contains the same entries and columns has ```PCode_Instructions.csv``` but also has some duplicate entries. It has a total of 5 293 entries.  
* ```PCode_Datasets.zip``` contains ```PCode_Instructions_Duplicates.csv``` and ```PCode_Instructions.csv```

# Usage

This dataset can be use to train a machine learning model to classify and detect malicious VBA macros from there P-Code instructions. 
After downloading the data, make sure to check their signatures for integrity purposes:

```
sigcheck -h PCode_Instructions.csv
  MD5:    555AC2E047B731D55D88BD98C03123DD
  SHA1:   55BA1392D365A016E13ECCDCEF551C03CD6BD9D6
  SHA256: 842C2CFB3F9D16E8275DBA5A0D2909957A91A14382857C6802A0491A7D4F60A8
  
sigcheck -h PCode_Instructions_Duplicates.csv
  MD5:    4D844B69056DA7E00C4FD2C36A40EB7F
  SHA1:   0322464268732490091503C3C61D5C0338D1B9D1
  SHA256: F36D10F793327A2CDF28A53C7AB6EAD2F4CF3754C684F36705C8E9D104F792DE
  
sigcheck -h PCode_Datasets.zip
  MD5:    82594CC3DF83A16F586387C57263A89A
  SHA1:   791228B9211BC8C08F519764F48140F44713CDA8
  SHA256: EF5000AD30039F47FD9E73EC3A0A6A0A026D18BADE3DDB231F59B3D212B5719D
```

# License

* The data is released under the terms of the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International  ](https://creativecommons.org/licenses/by-nc-sa/4.0/).
* The dataset is meant for research purposes.
