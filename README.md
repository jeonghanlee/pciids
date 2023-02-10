# pciids

When we run `lspci`, we can see pci device names there. The story behind is that many peoples update their interesting device name into a centralized db file by hand.

This effort helps a lot of Linux users' life easy. However, sometimes, the procedure needs a lot of time to spend that happens.

For big science facilities around world, typically, it is a painful effort to follow the private sector practices.

This repository was introduced to overcome this issue at least with minimum resouces and contains a few hardware PCIID database information. 

One can update the generic pci id file by the following commands


```
$ bash replace_pciids.bash

```
It will replace your local pciids with the repository pciids. 

The following hardware pciid defintions are in this repository.


## Micro-Research Finland Oy 

* http://www.mrf.fi/

```
1a3e  Micro-Research Finland Oy
	10c8  PMC Event Receiver 200
	11e6  PMC Event Receiver 230
	10dc  CPCI Event Receiver 220
	20dc  CPCI Event Generator 220
	10e6  CPCI Event Receiver 230
	20e6  CPCI Event Generator 230
	152c  CPCI Event Receiver 300
	172c  PCIE Event Receiver 300(DC)
	252c  CPCI Event Generator 300
	112c  PXIE Event Receiver 300
	212c  PXIE Event Generator 300
	192c  CPCI Event Receiver/Gun Transmitter 
	30e6  CPCI Fan-Out Concentrator
	132c  MTCA Event Receiver 300
	232c  MTCA Event Master 300
```


## Research Centre Juelich (Struck Innovative Systeme)

* http://www.struck.de/

```
1796  Research Centre Juelich
	0001  SIS1100 [Gigabit link]
	0002  HOTlink
	0003  Counter Timer
	0004  CAMAC Controller
	0005  PROFIBUS
	0006  AMCC HOTlink
	000d  Synchronisation Slave
	000e  SIS1100-eCMC
	000f  TDC (GPX)
	0010  PCIe Counter Timer
	0011  SIS1100-e single link
	0012  SIS1100-e quad link
	0015  SIS8100 [Gigabit link, MicroTCA]
	0018  SIS8300 [MicroTCA.4 digitizer]
	0019  SIS8300-L(2) [MicroTCA.4 digitizer]
	0024  SIS8300-KU [MicroTCA.4 digitizer]
```


### IOXOS Technologies SA

* https://www.ioxos.ch/

```
7357  IOxOS Technologies SA
	1001  PCIe EP No.0 - T2081
	1002  PCIe EP No.1 - AMC
	1003  PCIe EP No.2 - ADF
	7910  7910 [Althea]
```

### CAENels S.R.L.

* https://www.caenels.com/

```
cae2  CAENels S.R.L.
	71c0 CAENels MTCA AMC-PICO-8
	e551 CAENels MTCA DAMC-FMC25
```	
	
