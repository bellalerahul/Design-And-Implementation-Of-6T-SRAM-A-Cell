# Mini_project_1

ABSTRACT  
Static Random Access Memory (SRAM) is one of the core components in the digital world. Generally, it consumes enormous amount of power and die area. Thereby extensive research in SRAM is in progress related power dissipation, memory chip area and supply voltage requirement. In this paper SRAM analysis in terms of Static Noise Margin, Data Retention Voltage, Read Margin (RM) and Write Margin (WM) for low power application is considered. Static Noise Margin (SNM) is one of the most essential parameters for memory design because it affects both read and write margin. SNM is related to the threshold voltages of the Negative Metal Oxide Semiconductor (NMOS) and Positive Metal-Oxide Semiconductor (PMOS) devices of the SRAM cell. High Read and Write Noise Margin are also significant challenges in the design of SRAM. 
Performance analysis is estimated in 6T-SRAM designed and implemented using Cadence Virtuoso Tool


INTRODUCTION 
SRAM  is a type of Random Access Memory (RAM) that retains data bits in its memory as long as power is being supplied. Unlike Dynamic RAM (DRAM), which must be continuously refreshed, SRAM does not have this requirement, resulting in better performance and lower power usage. However, SRAM is also more expensive than DRAM, and it requires a lot more space. Stability in SRAM when designed using the Complementary Metal–Oxide– Semiconductor (CMOS) technologies generally depend on the SNM. SRAM memory technology is used because of its speed and robustness. As the device is scaled down in sizes several design challenges arise in the nanometre size SRAM design. In an SRAM cell operation generally supply voltage scaling is performed. Reducing the VDD reduces subthreshold leakage current and gate leakage. For analysing high speed SRAM calculation of read margin and WM is necessary.  Nowadays focus is on low supply voltage which reduces the SNM. The stability of SRAM cell can be analysed based on the SNM value because performance is proportional to the SNM.


LITERATURE SURVEY 

Soumya Gadag et al.,[1] Their research on the critical issue of power consumption reduction in VLSI (Very Large Scale 
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
Benton H. Calhoun et al.,[11] Discussing the importance of saving power in memory design develops, there is a trend to
functioning synapses at less available voltages. Investigations into sub-threshold operations for logic have revealed the possibility 
of low-energy operation in this region. This proposes a point of convergence for energy-constrained programmes, where SRAM 
can run at subthreshold voltages compatible with logic. Sub-threshold voltages, on the other hand, limit the static noise margin 
(SNM), making it critical to understand the impact of design decisions and other parameters. This article investigates SNM for 
sub-threshold bitcells in a 65-nm manipulate, looking at the impacts of size, DD, temperature, and threshold change. The findings 
show the large impact of variance on SNM and provide a methodology for estimating SNM throughout the most adverse 
distribution tail.
Gourav Arora et al.,[12] The challenge of establishing a high Read and Write Noise Margin in SRAM design is the topic of 
this study. It compares the read and write stability and ability of 6T and 7T SRAM cell architectures across technologies. The 
investigation focuses on the Static Noise Margin (SNM), which affects both the read and write margins. The article compares 
the Read Noise Margin (RNM) and Write Noise Margin (WNM) of both SRAM cell types in the paper. Using the Tanner EDA 
tool, the results reveal that the 7T SRAM cell outperforms the 6T SRAM cell by providing larger read and write noise margins 
across several CMOS technologies (45nm, 32nm, and 22nm). 
Arshad Moradi et al.,[13] Define a novel technique for increasing the margin of the 6T-SRAM cell in their study. The proposed 
method decreases the amount of space occupied by the subthreshold SRAM cell while enhancing its write cycle. This is 
accomplished by employing a PMOS-stacked network, which avoids the need for a write cycle.
Shweta Gupta et al.,[14] Focuses on minimizing leakage current in SRAM cells spanning various semiconductor technologies. 
The researchers investigate three source-biasing strategies to reduce power loss in the 6T SRAM device. These techniques 
involve the NMOS semiconductor clamping, PMOS diode securing and NMOS-PMOS diode clamp at 45 nm and 90 nm 
technology. Furthermore, the article highlights the fabrication of a 6T SRAM cell using the multiple threshold CMOS 
(MTCMOS) method at the 45 nm technology node. The simulations are run using supply voltages of 0.95 V and 0.45 V 
corresponding to the 90 nm and 45 nm technology, accordingly. The researchers hope to effectively reduce leakage current by 
investigating these strategies and technologies. 
Teijo Lehtonen et al.,[15] The focus of the study on using the Near-Threshold Computing (NTC) method to minimize power 
consumption in CMOS devices, specifically in the design of low-power cache memory circuits. Caches are known to consume 
a big amount of power and take up a significant amount of space in these kinds of systems, making their use of energy an 
important element in total system power efficiency. To solve this, the researchers examine the efficacy of 6T and 8T cells of
SRAM to determine which is best for cache memory circuits. According to the data, the 8T SRAM cell is more reliable than the 
6T SRAM cell. The paper intends to achieve considerable reductions by using NTC and selecting more trustworthy 8T SRAM 
cells. 
G. Shivaprakash et al.,[16] Research emphasizes the analysis of SRAM for applications that require little power, taking into 
account SRAM's critical position as a key component in the digital world. The paper specifically computes the Dramatic Read 
Voltage (DRV) for a 6T-SRAM cell optimized for high-speed applications. A 6T-SRAM design constructed in 90nm technology 
is subjected to performance study. SRAM is known for using a huge quantity of power and taking up an important portion of die
area. The Static Interference Margin (SNM) has been recognised as a significant characteristic in SRAM cells that affects both 
read and write margins. The threshold values of the NMOS and PMOS transistors within the SRAM cell are directly related to 
SNM. The researchers hope to learn more about these qualities by analyzing their paper.. 
Kavita Khare et al.,[17] Demonstrate the realization of a 6T SRAM cell that has shorter reading and writing times, region, and 
energy use. The researchers show that using greater cell ratios may improve read and write time while boosting stability. The
approach involves employing global bit lines to reduce energy use while increasing memory capacity. The study explicitly builds 
two SRAM cells for a 4 Kb storage core working at 1.8V supply voltage. However, it should be observed that increasing the 
capacity of memory also increases bit-line parasitic capacitance. This can lead to slower power sensing and higher energy 
consumption. By tackling these issues, scientists hope to improve the productivity and effectiveness of SRAM cells. 
Budhaditya Majumdar et al.,[18] Present a unique CMOS 6-transistor SRAM cell built primarily for independent and lowpower application in embedded systems. The suggested cell does not require a refresh cycle because it stores data via current
leaked and positive feedback. Surprisingly, the new cell is the same size as a normal six-transistor cell using identical techniques 
and design requirements. However, as compared to conventional architectures, it considerably improves energy consumption 
and read stability. This revolutionary CMOS 6-transistor SRAM cell offers a viable option for improving performance while 
remaining compact, making it suited for a wide range of low-power and mobile devices. 
Nahid Rahman et al.,[19] The issues experienced by static memory (SRAM) circuits owing to size decreased in System-OnChip (SoC) along with other integrated devices are explored in the study performed by Nahid Rahman, B. P. Singh et al. The 
requirement for better density in devices running at lower supply energies is driving the decrease of SRAM size. While this 
scaling allows for power savings, it has an influence on the performance and stability of SRAM circuits. The study, which 
focuses on the 45nm manufacturing node, gives vital insights to the stability difficulties and noise impacts experienced by 
traditional 6T SRAM cells as a result of supply voltage scaling. The study improves awareness of SRAM cell behavior and 
suggests potential techniques for improving safety during low-voltage operation. 
Hiroyuki Yamauch et al.,[20] This study examines the effects of various fin patterns on the electrical properties of hybrid 
Tunnel Field-Effect Transistors (TFETs) and assesses how well they function in comparison to hybrid TFETs with other fin 
shapes. The goal is to create fast, low-power devices for nanoelectronics technologies in the future. In comparison to 
traditional MOSFETs, TFET technology delivers greater leakage current reduction due to its tunnel switching capacity. The 
study examines the gate range of coverage of different fin designs with the goal of reducing leakage currents. Electrical 
properties for various fin shapes of TFETs, including drive current, leakage current, and subthreshold slope, are calculated 
using the TCAD simulation programme. This shows TFETS functions better.

METHODOLOGY
Design the SRAM cell schematic. This involves drawing the schematic of the 6T SRAM cell, including the two inverters, the two access transistors, and the bit lines.
Simulate the SRAM cell. This involves simulating the operation of the SRAM cell using the Cadence Virtuoso simulator. The simulation should verify that the SRAM cell can store and retrieve data correctly.
Layout the SRAM cell. This involves laying out the SRAM cell in a physical design environment. The layout should be optimized for area, power, and performance.
Implement the SRAM cell. This involves generating the layout data for the SRAM cell and placing it in a larger design.
Simulate the SRAM array. This involves simulating the operation of the entire SRAM array using the Cadence Virtuoso simulator. The simulation should verify that the SRAM array can store and retrieve data correctly.
Place and route the SRAM array. This involves placing the SRAM array in a larger design and routing the connections between the SRAM cells.
Generate the final design file. This involves generating the final design file that can be used to fabricate the SRAM chip.
![aa](https://github.com/bellalerahul/Mini_project_1/assets/93982029/a1bee354-1c83-41b3-8c03-382d28c5b8e6)

REFERENCES

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
[6]6.Manoj Padmanabha Murthy. T1, Nithin. N 2, Pallavi. N 3, V. Rajashekar4, Sharanagouda. V Patil5,“Performance 
Analysis of SRAM at Different Technologies using Cadence”,ISSN 2321 3361 © 2020 IJESC.
[7] 7.Changhwan Shin,“Performance and Area Scaling Benefits of FD-SOITechnology for 6-T SRAM Cells at the 
22-nm Node”,IEEE TRANSACTIONS ON ELECTRON DEVICES, VOL. 57, NO. 6, JUNE 2010.
[8]Rajasekhar Keerthi and Chein-in Henry Chen,“Stability and Static Noise Margin Analysis of Low-Power 
SRAM”,I2MTC 2008 - IEEE International Instrumentation and Measurement Technology Conference Victoria, 
Vancouver Island, Canada, May 12-15, 2008.
[9]Christiensen D.C. Arandilla, Anastacia B. Alvarez, and Christian Raymund K. Roque,“
Static Noise Margin of 6T SRAM Cell in 90-nm CMOS”, UKSim 13th International Conference on Modelling and 
Simulation,2011.
[10]Panduranga Vemula,S. Priyanka, M. Raheez, A. Sairam,“Design and Analysis of 6T SRAM in 45NM”, 
TechnologyInternational Journal of Engineering Research & Technology (IJERT) Vol. 11 Issue 05, May-2022.
[11]11.Benton H. Calhoun,Anantha P. Chandrakasan,“Static Noise Margin Variation for Sub-threshold SRAM in 
65-nm CMOS”,IEEE JOURNAL OF SOLID-STATE CIRCUITS, VOL. 41, NO. 7, JULY 2006.
[12].Gourav Arora1, Poonam2, Anurag Singh3,“SNM Analysis of Sram Cells at 45nm, 32nm and 22nm 
Technology”,International Journal of Engineering Research and General Science Volume 2, Issue 4, June-July, 
2014 ISSN 2091-2730.
[13].Farshad Moradi1, Dag T. Wisland1, Hamid Mahmoodi2, Tuan Vu Cao ,“Improved Write Margin 
6T-SRAM for Low Supply Voltage Applications”,978-1-4244-4941-1-5/09/$25.00,2009,IEEE.
[14] Sufia Banu1 and Shweta Gupta2,“Design and Leakage Power Optimization of 6T Static 
Random Access Memory Cell Using Cadence Virtuoso “,International Journal of Electrical and 
Electronics Research (IJEER)Research Article | Volume 10, Issue 2 | Pages 341-346 | e-ISSN: 2347-470X.
[15]Mika Kutila, Ari Paasio and Teijo Lehtonen,“Comparison of 130 nm Technology 6T and 8T SRAM 
Cell Designs for Near-Threshold Operation”,978-1-4799-4132-2/14/$31.00 ©2014 IEEE.
[16]G. Shivaprakash1* and D. S. Suresh2,“Design of Low Power 6T-SRAM Cell and Analysis for High 
“Speed Application”,Indian Journal of Science and Technology”, Vol 9(46),December 2016.
[17]Kavita Khare 1 , Nilay Khare2 , Vijendra Kumar Kulhade3 , Pallavi Deshpande4,“VLSI Design And 
Analysis OfLow Power 6T SRAM Cell Using Cadence Tool”,lCSE 2008 Proc.2008, lohor Bahru, 
Malaysia.
[18]Budhaditya Majumdar,Sumana Basu,“Low Power Single Bitline 6T SRAM Cell With High Read 
Stability”,2011 International Conference on Recent Trends in Information Systems.
[19]Nahid Rahman,B. P. Singh,“Static-Noise-Margin Analysis of Conventional 6T SRAM Cell at 45nm 
Technology”,International Journal of Computer Applications (0975 – 8887) Volume 66– No.20, March
[20]Hiroyuki Yamauchi, “A Discussion on SRAM Circuit Design Trend in Deeper Nanometer-Scale Technologies”,
IEEE TRANSACTIONS ON VERY LARGE SCALE INTEGRATION (VLSI) SYSTEMS, VOL. 18, NO. 5, MAY 2010

