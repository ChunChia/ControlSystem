ControlSystem
=============
![alt tag](https://cloud.githubusercontent.com/assets/4612912/5442403/40bcf874-8499-11e4-805a-2139ef6d2299.png)

adding a analog output looks like below
```
        for (int j=0;j<8;j++) MultiIO->AddAnalogOut(Bus1+104+j); //ana 8..15;
        ```
Each MultiIO->AddAnalogOut command adds an analog output to the MultiIO system.
