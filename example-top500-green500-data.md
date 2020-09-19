```
Submissions ID: 8f442200-3a90-4bc7-b1c5-fb83d8caf302

MIT/MGHPCC Holyoke, MA

Actual Site Name	MIT/MGHPCC Holyoke, MA
Site URL	https://researchcomputing.mit.edu
Acronym	MIT
Segment	Academic
City	Holyoke
Country	United States of America
Satori

Installation Date	Sept. 24, 2019
System URL	https://researchcomputing.mit.edu/satori
Applications Area	Research
Vendor	IBM
Component 1: Satori

Model	AC922
Nodes	64
Vendor	IBM
Processor	IBM Power 9 20C 2.4GHz
Speed	2400
Sockets per Node:	2
Cores per Socket:	20
Accelerator/CP:	Tesla V100-SMX2-32GB
Accelerators/CP per Node:	4
Cores per Accelerator/CP:	80
Operating System:	RHEL 7.6
Primary Interconnect:	Infiniband EDR
Peak Power (kW):	105.04
Size of Power Measurement (Cores)	23040
Memory per Node (GB)	1024
Summary of all components

CPU Cores	2560
Accelerators/CP	256
Accelerator/CP Cores	
Memory	65536 GB
Power	105.04 kW
Linpack Benchmark

Benchmark Date	Oct. 22, 2019
CPU Cores	2560
Accelerator/CP Cores	20480
Rmax	1562.00 GFlop/s
Rpeak	1996.00 GFlop/s
Nmax	2555904
Nhalf	None
```

HPL input
```
HPLinpack benchmark input file
Innovative Computing Laboratory, University of Tennessee
HPL.out      output file name (if any)
6            device out (6=stdout,7=stderr,file)
1            # of problems sizes (N)
2555904 2588160  110592  622080 1244160 2488320 2592768 1769472 1543680  311040   Ns
1            # of NBs
768         NBs
0            PMAP process mapping (0=Row-,1=Column-major)
1            # of process grids (P x Q)
16 4 8 16         Ps
16 2 8 16         Qs
16.0         threshold
1            # of panel fact
2 2 2        PFACTs (0=left, 1=Crout, 2=Right)
1            # of recursive stopping criterium
4 4 4        NBMINs (>= 1)
1            # of panels in recursion
2            NDIVs
1            # of recursive panel fact.
0 0 0        RFACTs (0=left, 1=Crout, 2=Right)
1            # of broadcast
3 1          BCASTs (0=1rg,1=1rM,2=2rg,3=2rM,4=Lng,5=LnM)
1            # of lookahead depth
0            DEPTHs (>=0)
1            SWAP (0=bin-exch,1=long,2=mix)
768          swapping threshold
1            L1 in (0=transposed,1=no-transposed) form
0            U  in (0=transposed,1=no-transposed) form
0            Equilibration (0=no,1=yes)
8            memory alignment in double (> 0)
```

Power information

- in power measurements below (line beginning Power Comments	Samples of average power every 180 ) the fields are "date time","timestamp","power" where power is in Watts. So typical power for this benchmark was 106KJ/s.  
```
Software

Compiler	NVidia Binary
Compiler Options used	
Math Library	
MPI Library	IBM Spectrum MPI
Power

Power Level	2
Power Comments	Samples of average power every 180 secs from Revenue Grade Meter. CSV of measurements is shown below. Timestamp,Average Power(W) 2019-10-22 10:46:00 1571755560,106440 2019-10-22 10:49:00 1571755740,106284 2019-10-22 10:52:00 1571755920,106487 2019-10-22 10:55:00 1571756100,106540 2019-10-22 10:58:00 1571756280,106532 2019-10-22 11:01:00 1571756460,105599 2019-10-22 11:04:00 1571756640,105794 2019-10-22 11:07:00 1571756820,106009 2019-10-22 11:10:00 1571757000,105446 2019-10-22 11:13:00 1571757180,106094 2019-10-22 11:16:00 1571757360,106203 2019-10-22 11:19:00 1571757540,105630 2019-10-22 11:22:00 1571757720,105494 2019-10-22 11:25:00 1571757900,106194 2019-10-22 11:28:00 1571758080,106003 2019-10-22 11:31:00 1571758260,104041 2019-10-22 11:34:00 1571758440,92724 2019-10-22 11:37:00 1571758620,105255 2019-10-22 11:40:00 1571758800,105573 2019-10-22 11:43:00 1571758980,104891 2019-10-22 11:46:00 1571759160,103697 2019-10-22 11:49:00 1571759340,105667 2019-10-22 11:52:00 1571759520,105582 2019-10-22 11:55:00 1571759700,105619 2019-10-22 11:58:00 1571759880,105150 2019-10-22 12:01:00 1571760060,104102 2019-10-22 12:04:00 1571760240,105092 2019-10-22 12:07:00 1571760420,104927 2019-10-22 12:10:00 1571760600,105066 2019-10-22 12:13:00 1571760780,105407 2019-10-22 12:16:00 1571760960,105334 2019-10-22 12:19:00 1571761140,105127 2019-10-22 12:22:00 1571761320,105350 2019-10-22 12:25:00 1571761500,104933 2019-10-22 12:28:00 1571761680,105444 2019-10-22 12:31:00 1571761860,102916 2019-10-22 12:34:00 1571762040,104365 2019-10-22 12:37:00 1571762220,104614
Peak Power	105.00
Measured Cores	23040
Measure Device	Measurelogic DTS310 Revenue Grade Meters
Measure Date	Oct. 22, 2019
Cooling on	False
Storage on	False
```
HPL output
```
```
