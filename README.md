# DetectionData

Unprocessed detections data from project tags and receivers

Shield: [![CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](http://creativecommons.org/licenses/by-sa/4.0/)

The following data files are presented in this repository

```{=native}
Receivers/2022_TaggingReceiver_SG-4493RPI39F52.motus.csv
Receivers/2023_TaggingReceiver_SG-4FA8RPI31938.motus.csv
Receivers/Bedfont_CTT-DFA627A74176.motus.csv
Receivers/Benacre_SG-2C25RPI3D464.motus.csv
Receivers/Dungeness_SG-3847RPI3BD14.motus.csv
Receivers/Eccles_CTT-1610F6693478.motus.csv
Receivers/FB_TestReceiver_SG-EFCCRPI30456.motus.csv
Receivers/FoulnessNorth_CTT-V30B0154DF58.motus.csv
Receivers/GibraltarPoint_CTT-V3023D0E2535.motus.csv
Receivers/PortlandBirdObs_CTT-V30B0154B9A9.motus.csv
Receivers/Receiver_not_deployed_CTT-FCDA961032DB.motus.csv
Receivers/SandwichBay_SG-8518RPI36527.motus.csv
Receivers/SouthendPier_CTT-V30B0154CA8C.motus.csv
Receivers/Spurn_SG-3206RPI30D24.motus.csv
Receivers/StanfordReservoir_CTT-6A35DE207818.motus.csv
Receivers/TestReceiver_SG-DA1ARPI3C11C.motus.csv
Receivers/TheDeep_CTT-77C282B0581A.motus.csv
Receivers/TophillLow_CTT-97B20FBE69BF.motus.csv
Receivers/Weybourne_CTT-98A5D0BB4E1D.motus.csv
Receivers/Wheldrake_CTT-AD554C13AB19.motus.csv
Tags/project-291.motus.csv
Tags/project-307.motus.csv
```
To import a file into R use the function `read_csv()` from the Tidyverse package.

You will need to prepend the following file path "<https://raw.githubusercontent.com/Motus-307/DetectionData/main/>"

The following example shows how to download the data file for the Eccles_CTT receiver

``` r
library(tidyverse)

remote_file <- "Receivers/Eccles_CTT-1610F6693478.motus.csv"
#Change the above to match whichever file you want to download

remote_path <- "https://raw.githubusercontent.com/Motus-307/DetectionData/main/"
#This shouldn't need to change

my_tbl <- read_csv(paste0(remote_path,remote_file))
```

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).

[![CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/88x31.png)](http://creativecommons.org/licenses/by-sa/4.0/)
