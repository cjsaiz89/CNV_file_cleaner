# CNV_file_cleaner

The script "cleans" the cruiseid_time_stationN.cnv file from the CTD and cruiseid_profile_stationN.cnv, replacing bad-flagged values by the value from the previous line. It creates a _backup file, and renames the original file with extension _ORIGINAL, in case some unexpected error comes up in the middle of the execution.

In case the script is executed twice, and the *cnv to clean is not the original, it will detect the existence of the _ORIGINAL and skip the process.

A log file is created (cruiseIDcnv_cleaner.log), to log every execution showing date-time and lines changed.

> python CNV_cleaner.py
> ** CTD .cnv cleaner **
> 
> 
> Enter CTD station [xxx]:996
> 
> PNE2021b_profile_996.cnv backed up as PNE2021b_profile_996.cnv_backup
> PNE2021b_time_996.cnv backed up as PNE2021b_time_996.cnv_backup
>  
> 0 lines were replaced in PNE2021b_profile_996.cnv
> 
> PNE2021b_profile_996.cnv renamed as PNE2021b_profile_996.cnv_ORIGINAL
> temp_PNE2021b_profile_996.cnv renamed as PNE2021b_profile_996.cnv
> PNE2021b_profile_996.cnv processed
> 
> 
> Replace -9.990e-29 position 4 by 9.8505
> Replace -9.990e-29 position 5 by 9.8516
> Replace -9.990e-29 position 4 by 4.8131
> Replace -9.990e-29 position 5 by 4.8128
> Replace -9.990e-29 position 4 by 7.2602
> Replace -9.990e-29 position 3 by 708.811
> Replace -9.990e-29 position 5 by 16.4331
> Replace -9.990e-29 position 15 by 4.9993
> Replace -9.990e-29 position 3 by 6.375
> Replace -9.990e-29 position 15 by 4.0826
> Replace -9.990e-29 position 12 by 3.0040
> Replace -9.990e-29 position 13 by 2.7502
> Replace -9.990e-29 position 14 by 5.9134
> Replace -9.990e-29 position 15 by 4.9808
> 9 lines were replaced in PNE2021b_time_996.cnv
> 
> PNE2021b_time_996.cnv renamed as PNE2021b_time_996.cnv_ORIGINAL
> temp_PNE2021b_time_996.cnv renamed as PNE2021b_time_996.cnv
> PNE2021b_time_996.cnv processed
> 
> 
> 
> 
> ** Process finished **
> 
> Proceed with process_cast xxx
