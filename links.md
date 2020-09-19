# Some links to material for ideas/inspiration!

# Green 500 systems
Every 6 months some lists 
https://www.top500.org/lists/top500/, https://www.top500.org/lists/green500/ are published of the fastest computers in the world. 
These lists include information on where the computers are, how fast they ran a benchmark calculation and how much power
they used when running the benchmark.

# Exploring some green algorithm and energy ideas
https://news.mit.edu/2020/brainstorming-energy-saving-hacks-satori-mit-supercomputer-0211
https://news.mit.edu/2020/shrinking-deep-learning-carbon-footprint-0807
https://www.youtube.com/watch?v=Vrc1H4xSH7o&feature=youtu.be

# Energy source generation mix
Depending on a computers location it may take energy from more or less CO2 emiting generators. 
This page show how energy source vary state by state in the US https://www.eia.gov/electricity/data/state/.

# Energy mix of specific data centers
For some facilities you can find more detailed information on their local energy source CO2 emissions. For example, this
page https://www.hged.com/community-environment/green%20initiative/our-energy-mix.aspx shows the enrgy mix for these
facilities https://www.mghpcc.org, https://www.ll.mit.edu/r-d/cyber-security-and-information-sciences/lincoln-laboratory-supercomputing-center
in the Top 500 list. A sense of the global mix of energy sources can be read from here, https://www.carbonbrief.org/mapped-worlds-coal-power-plants. 


# Data center locations
Have you ever wondered physically where the cloud is. This site https://www.datacenters.com/locations is great for figuring out where the hardware is and what energy mix 
it is using. 

# Prior art
Here is a site https://mlco2.github.io/impact/#home where you can calculate a Machine Learning CO2 estimate. Its not that exciting, but it does have some useful information. No nice images, no music, not a lot of detail etc.... 

# What about data center energy efficiency
In some data centers 50% of the energy used is going toward keeping computers cool, in others it is less than 15%. This is called Power Usage Efficiency (PUE) and it can vary between sites. This is a fun site https://www.nrel.gov/computational-science/measuring-efficiency-pue.html with a dashboard that talks about PUE at a datacenter in Colarado, US. More information on PUE is linked through here https://en.wikipedia.org/wiki/Power_usage_effectiveness .

# What about time of day or day of week
At some times on some days you may be more likely to cause a CO2 emiting gas turbine to come online https://www.sciencedirect.com/science/article/pii/S2214629616302985?via%3Dihub . What are good ways to convey that. 

# What about time of year and weather
Data centers typically need more cooling energy when it is hot and humid. Could we encourage everyone to use data centers
in Iceland https://www.ibm.com/blogs/nordic-msp/iceland-data-centers/. 


# How should we show CO2 emissions.
What does 150 tons of coal look like - https://www.agefotostock.com/age/en/Stock-Images/Rights-Managed/X2J-1279992. How much CO2 is that ( 1 x C12 + 2 x O8 ).
What about a tree https://www.unm.edu/~jbrink/365/Documents/Calculating_tree_carbon.pdf , how many trees is 1MT of CO2? 

# Is there a useful calculator to help me
Yes this site https://www.epa.gov/energy/greenhouse-gas-equivalencies-calculator has useful formulae. 

# How do I convert between Kg of gasoline and Kg CO2. 
Molecular weights of the representative octane combustion are C8H18 114, O2 32, CO2 44, H2O 18; therefore 1 kg of fuel reacts with 3.51 kg of oxygen (from the atmosphere) to produce 3.09 kg of carbon dioxide and 1.42 kg of water ( see -  https://en.wikipedia.org/wiki/Gasoline ). 

# Algorithms and hardware also matter
Here is a paper http://www.netlib.org/utk/people/JackDongarra/PAPERS/haidar_fp16_sc18.pdf where they used BFloat16 arithmetic to save energy.
The energy use of a floating point computation goes as the square ot the number of mantissa bits ( https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.95.5235&rep=rep1&type=pdf ). 

# Measuring power on a computer
Most computers have base board management controller (BMC) that can be queried https://en.wikipedia.org/wiki/OpenBMC .
Satori uses something called Witherspoon - that is based on https://github.com/openbmc/openbmc .
For metering power to racks Satori has ```Measurelogic DTS310 Revenue Grade Meters``` ( https://www.measurlogic.com/wp-content/uploads/2017/01/DTS-310-5.pdf ).

# What is a carbon offset
This link explains a bit about carbon offsets https://www.terrapass.com/climate-change/carbon-offsets-explained . It lets you buy some too if you
want to offset your CO2 emissions!

# How should I think about overall greenhouse gas emissions
Good question! This site https://ghgprotocol.org has some ideas on approaches that have been used to try and think about end-to-end emissions. Where to start and 
where to end is inevitably a little bit of a judgement. 

# How many floating point operations does a typical computation use
The Top 500 computation (Linpack) has a certain floating point operationcount that can be understood from the Top 500 spreadsheet. The 
count is fairly strongly linked with energy use. This article 
https://iq.opengenus.org/floating-point-operations-per-second-flops-of-machine-learning-models/ gives a sense of a typical 
machine learning code. 
