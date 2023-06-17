# Mini_project_1

# ABSTRACT  
Static Random Access Memory (SRAM) is one of the core components in the digital world. Generally, it consumes enormous amount of power and die area. Thereby extensive research in SRAM is in progress related power dissipation, memory chip area and supply voltage requirement. In this paper SRAM analysis in terms of Static Noise Margin, Data Retention Voltage, Read Margin (RM) and Write Margin (WM) for low power application is considered. Static Noise Margin (SNM) is one of the most essential parameters for memory design because it affects both read and write margin. SNM is related to the threshold voltages of the Negative Metal Oxide Semiconductor (NMOS) and Positive Metal-Oxide Semiconductor (PMOS) devices of the SRAM cell. High Read and Write Noise Margin are also significant challenges in the design of SRAM. 
Performance analysis is estimated in 6T-SRAM designed and implemented using Cadence Virtuoso Tool


# INTRODUCTION 
SRAM  is a type of Random Access Memory (RAM) that retains data bits in its memory as long as power is being supplied. Unlike Dynamic RAM (DRAM), which must be continuously refreshed, SRAM does not have this requirement, resulting in better performance and lower power usage. However, SRAM is also more expensive than DRAM, and it requires a lot more space. Stability in SRAM when designed using the Complementary Metal–Oxide– Semiconductor (CMOS) technologies generally depend on the SNM. SRAM memory technology is used because of its speed and robustness. As the device is scaled down in sizes several design challenges arise in the nanometre size SRAM design. In an SRAM cell operation generally supply voltage scaling is performed. Reducing the VDD reduces subthreshold leakage current and gate leakage. For analysing high speed SRAM calculation of read margin and WM is necessary.  Nowadays focus is on low supply voltage which reduces the SNM. The stability of SRAM cell can be analysed based on the SNM value because performance is proportional to the SNM.


# LITERATURE SURVEY 

* Soumya Gadag et al.,[1] Their research on the critical issue of power consumption reduction in VLSI (Very Large Scale 
Integration). To reduce power loss, they used strategies like sleep and stacking. The design was developed using 0.18um CMOSbased technology, and the power dissipation was assessed using the microwind tool at the BSIM4 level.Surprisingly, their 
technique yielded a notable 40% reduction in overall power dissipation when compared to the typical 6T SRAM cell. This 
reduction in power usage is an important development in VLSI design since it leads to greater energy efficiency and battery life 
in electronic products. The study's findings emphasize the usefulness of their method in minimizing power-related difficulties 
and improving overall performance. 

Michael C. Wang et al.,[2] Proposed a paradoxical method for lowering power consumption for SRAM operations. They
advocated employing two distinct word lines (WL) as well as one WL linked to the cell's transistor. This technology aims to
reduce switching power on the word line (WL) and bit line (BL), resulting in lower overall power consumption. The success of 
this strategy was proven by simulated outputs, which showed a considerable reduction in power consumption when using two 
WLs in SRAM operations. Their technique, which optimizes the switching strategy and reduces power dissipation, has the
potential to improve energy efficiency in SRAM designs and the overall performance of memory systems. Their study's findings 
help to continue attempts to reduce electricity uses.

Michel Stuchi et al.,[3] This paper evaluated the read stability of the N curve metrics with the Static Noise Margin (SNM) in
their study. The write ability was also compared using N curve measurements and standard approaches. Analytical methods were 
created to evaluate these indicators.According to the findings, VDD scaling did not interfere with read stability. The output of 
the N curve metrics was compared to both worst-case and corner-case designs. The study sought to assess the efficacy of N curve 
metrics in terms of read stability and write ability.The findings emphasized the benefits of employing N curve parameters to 
evaluate read stability and write capabilities in SRAM architectures. Using analytical techniques.

Akshay Bhaskar et al.,[4] Research was to reduce power consumption and delay in SRAM write operations. They used two
approaches to do this: Gated VDD and MTCMOS. Their research found that the MTCMOS technology reduced power usage by 
38.1% when compared to standard 6T SRAM. It also improved speed by 18.18%. In comparison to the typical 6T SRAM, the 
Gated VDD design consumed 16.18% less power and performed 13.03% faster.These findings illustrate the effectiveness of 
both strategies in decreasing power consumption and enhancing performance in SRAM write operations. The deployment of 
Gated VDD and MTCMOS gives valuable strategies.

Mukesh Kumar et al.,[5] Reviewed and compared 6T, 7T, and 8T SRAM cells using the gpdk180 technology. The study aimed 
to examine various parameters such as dynamic and static power, rise and fall time, delay, and bandwidth. The Cadence tool was 
used for the analysis.The study discovered that the static power consumption was the same for all three SRAM cell designs. 
However, the dynamic power consumption for the 7T SRAM was found to be 5.45uW and 10.26uW for the 8T SRAM, indicating 
that the 8T configuration consumes more power. The experiments were carried out at a temperature of 27°C.These findings shed 
light on the trade-offs between power consumption and performance for various SRAM cell designs. Researchers and designers 
can improve their results by evaluating these parameters.

Manoj Padmanabha Murthy. T et al.,[6] This thesis investigates and compares the design and performance of SRAM cells in 
180nm and 45nm technologies. SRAM is a high-speed semiconductor memory that uses bistable circuits to store 1 bit of data 
and does not require refresh circuits like DRAM. Because of its fast data access, it is often employed as cache memory in
processors and controllers. DRAM, as opposed to SRAM, is denser and is utilized in major memories where speed is less
important. SRAM is finding new uses in industrial and automotive electronics. The thesis is concerned with reducing area by
proposing compact layouts for peripherals such as pre-charge and sensing amplifiers. PVT analysis is used to assess the durability 
of the SRAM cell to modifications and to notice power fluctuations. Furthermore, the power values are compared when the 
width of the channel is doubled or tripled.

Changhwan Shin et al.,[7] The efficiency and threshold voltage variability of completely depleted silicon-on-insulator (FDSOI) MOSFETs are compared to conventional bulk MOSFETs in this study. The authors examine the characteristics of these 
two types of MOSFETs using 3-D device modeling with atomistic doping profiles. The operating measurements of a sixtransistor SRAM cell at the 22 nm CMOS semiconductor node are then estimated using compact modeling. The research looks 
at how cell ratio, pull-up ratio, and operating voltage affect read and write margins as well as read current in FD-SOI and bulk 
SRAM cells. The yield and cell-area advantages of FD-SOI technology are investigated using iso-area and iso-yield
comparisons. Furthermore, the study compares the minimum operating voltages (Vmin) required for FD-SOI and bulk SRAM
cells to meet.

Rajasekhar Keerthi et al.,[8] In this research, a seven-transistor (7T) SRAM cell is used and compared to a typical six-transistor 
(6T) SRAM cell to address read data destruction and improve stability at IOW-VDD. The solid functioning of an 8-bit SRAM, 
also known, is demonstrated using statistical model and data analysis, taking into account variations in the process and mismatch. 
The measurement results indicate that the stationary noise margin (SNM) of the 7T SRAM cell matches that of the 6T SRAM 
cell. In addition, the stability of the 8-bit 7T SRAM at IOW-VDD has been demonstrated by properly testing the SRAM at 720 
mV, which highlights its improved reliability and performance over the 6T SRAM. 

Christensen D.C. et al.,[9] This article studies the Static Noise Margin (SNM) of a 6T Static Random Access Memory (SRAM) 
cell developed in 90-nm CMOS technology. The research entails modeling the SRAM cell and analyzing the noise margins 
while adjusting various parameters that influence SRAM operations. Temperature, threshold voltage, power supply voltage, cell 
ratio, pull-up ratio, and the process corner changes are among the parameters. The results of the simulation are compared to the 
square law device concept given by Seevinck . The study's findings show that the computer simulation results match the model, 
proving the model's validity in predicting the behavior of the SRAM cell under various operating situations. This study adds to 
our understanding of and optimisation of 6T SNM.

Panduranga Vemula et al.,[10] Reviewed in detail about increased use of SRAM and CMOS technology in processors and
system-on-a-chip (SoC) devices, new design innovations are necessary for SRAM to keep up with scaling. SRAM bit cells,
which are made up of the smallest geometric devices, seek for high density but are sensitive to technical scaling. The successful 
implementation of SRAM is critical to the success of future technologies. Several SRAM bitcell topologies and array layouts 
have been proposed to address concerns such as poor stability, process variation tolerance, device aging, and soft errors. This 
chapter addresses the function of SRAM in current computer systems, peripheral circuitries, and various SRAM bitcell 
topologies, as well as their benefits and drawbacks.


# METHODOLOGY
Schematic for designing the SRAM cell. This includes drawing of a 6T SRAM cell containing two inverters, two input transistors and a bit line. emulates a SRAM cell. This is to simulate SRAM cell operation using the Cadence Virtuoso simulator. The simulation must ensure that the SRAM cells can properly store and store data.SRAM cell layout. This includes placing SRAM cells in onboard physical space. The layout should be optimized for space, power and performance. The uses SRAM cells. This involves creating a data layout for SRAM cells and embedding them in a larger design.Simulates the SRAM array. This is an attempt to simulate the entire SRAM array using the Cadence Virtuoso simulator. The simulation must ensure that the SRAM array can properly store and store data. Location and orientation of SRAM arrays. This involves placing the SRAM array in a larger design and connecting the SRAM cells.Create the final design file. This includes the creation of final design files that can be used to build SRAM chips.
 
 ![aa](https://github.com/bellalerahul/Mini_project_1/assets/93982029/a1bee354-1c83-41b3-8c03-382d28c5b8e6)

# REFERENCES

[1] 1.Soumya Gadag*, Raviraj D.Chougala*,“Design and Analysis of 6T SRAM Cell with low Power Dissipation”, 
(IJERA) ISSN: 2248-9622 Vol. 2, Issue 6, November- December 2012, pp.1695-1698.
[2]Michael C. Wang,“Low Power Dual Word Line 6-Transistor SRAMs”,Roceedings of the World Congress on 
Engineering and Computer Science 2009 Vol I WCECS 2009, October 20-22, 2009/, San Francisco, USA,’.
[3] Evelyn Grossar, Michele Stucchi, Karen Maex, Member, IEEE,”Read Stability and Write-Ability Analysis 
ofSRAM Cells for Nanometer Technologies”,IEEE JOURNAL OF SOLID-STATE CIRCUITS, VOL. 41, NO. 11, 
NOVEMBER 2006.
[4] 4.Akshay Bhaskar,“Design and Analysis of Low Power SRAM Cells”,International Conference on Innovations in 
Power and Advanced Computing Technologies [i-PACT2017].
[5]Mukesh Kumar,Jagpal Singh Ubhi ,“Performance Evaluation of 6T, 7T & 8T SRAM at 180 nm Technology” ,8th 
ICCCNT 2017 July 3 - 5, 2017, IIT Delhi, Delhi, India.


