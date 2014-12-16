ControlSystem
=============
![alt tag](https://cloud.githubusercontent.com/assets/4612912/5442403/40bcf874-8499-11e4-805a-2139ef6d2299.png)

adding an code for analog output looks like below

```for (int j=0;j<8;j++) MultiIO->AddAnalogOut(Bus1+104+j); //ana 8..15;```

Each MultiIO->AddAnalogOut command adds an analog output to the MultiIO system.Each analog output
card contains eight analog outputs with eight consecutive addresses.(In the new rack version analog output, the output number is 4), in that case, you have to change the code to something like

```for (int j=0;j<4;j++)...```

Therefor, the number given has to be a multiple of four.

```AddAnalogOut(BusX+104+j) ```

the BusX species the subbus number by the dip switches in the BUS driver card with subbus decoder. Here, 104 is just an example of the hardware address set on the analog output board.   
