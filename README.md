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

* Michael C. Wang et al.,[2] Proposed a paradoxical method for lowering power consumption for SRAM operations. They
advocated employing two distinct word lines (WL) as well as one WL linked to the cell's transistor. This technology aims to
reduce switching power on the word line (WL) and bit line (BL), resulting in lower overall power consumption. The success of 
this strategy was proven by simulated outputs, which showed a considerable reduction in power consumption when using two 
WLs in SRAM operations. Their technique, which optimizes the switching strategy and reduces power dissipation, has the
potential to improve energy efficiency in SRAM designs and the overall performance of memory systems. Their study's findings 
help to continue attempts to reduce electricity uses.

* Michel Stuchi et al.,[3] This paper evaluated the read stability of the N curve metrics with the Static Noise Margin (SNM) in
their study. The write ability was also compared using N curve measurements and standard approaches. Analytical methods were 
created to evaluate these indicators.According to the findings, VDD scaling did not interfere with read stability. The output of 
the N curve metrics was compared to both worst-case and corner-case designs. The study sought to assess the efficacy of N curve 
metrics in terms of read stability and write ability.The findings emphasized the benefits of employing N curve parameters to 
evaluate read stability and write capabilities in SRAM architectures. Using analytical techniques.

* Akshay Bhaskar et al.,[4] Research was to reduce power consumption and delay in SRAM write operations. They used two
approaches to do this: Gated VDD and MTCMOS. Their research found that the MTCMOS technology reduced power usage by 
38.1% when compared to standard 6T SRAM. It also improved speed by 18.18%. In comparison to the typical 6T SRAM, the 
Gated VDD design consumed 16.18% less power and performed 13.03% faster.These findings illustrate the effectiveness of 
both strategies in decreasing power consumption and enhancing performance in SRAM write operations. The deployment of 
Gated VDD and MTCMOS gives valuable strategies.

* Mukesh Kumar et al.,[5] Reviewed and compared 6T, 7T, and 8T SRAM cells using the gpdk180 technology. The study aimed 
to examine various parameters such as dynamic and static power, rise and fall time, delay, and bandwidth. The Cadence tool was 
used for the analysis.The study discovered that the static power consumption was the same for all three SRAM cell designs. 
However, the dynamic power consumption for the 7T SRAM was found to be 5.45uW and 10.26uW for the 8T SRAM, indicating 
that the 8T configuration consumes more power. The experiments were carried out at a temperature of 27°C.These findings shed 
light on the trade-offs between power consumption and performance for various SRAM cell designs. Researchers and designers 
can improve their results by evaluating these parameters.

# METHODOLOGY
Schematic for designing the SRAM cell. This includes drawing of a 6T SRAM cell containing two inverters, two input transistors and a bit line. emulates a SRAM cell. This is to simulate SRAM cell operation using the Cadence Virtuoso simulator. The simulation must ensure that the SRAM cells can properly store and store data.SRAM cell layout. This includes placing SRAM cells in onboard physical space. The layout should be optimized for space, power and performance. The uses SRAM cells. This involves creating a data layout for SRAM cells and embedding them in a larger design.Simulates the SRAM array. This is an attempt to simulate the entire SRAM array using the Cadence Virtuoso simulator. The simulation must ensure that the SRAM array can properly store and store data. Location and orientation of SRAM arrays. This involves placing the SRAM array in a larger design and connecting the SRAM cells.Create the final design file. This includes the creation of final design files that can be used to build SRAM chips.
 
 ![aa](https://github.com/bellalerahul/Mini_project_1/assets/93982029/a1bee354-1c83-41b3-8c03-382d28c5b8e6)

 
# REFERENCES
* [1]Soumya Gadag*, Raviraj D.Chougala*,“Design and Analysis of 6T SRAM Cell with low Power Dissipation”, 
(IJERA) ISSN: 2248-9622 Vol. 2, Issue 6, November- December 2012, pp.1695-1698.

* [2]Michael C. Wang,“Low Power Dual Word Line 6-Transistor SRAMs”,Roceedings of the World Congress on 
Engineering and Computer Science 2009 Vol I WCECS 2009, October 20-22, 2009/, San Francisco, USA,’.

* [3] Evelyn Grossar, Michele Stucchi, Karen Maex, Member, IEEE,”Read Stability and Write-Ability Analysis 
ofSRAM Cells for Nanometer Technologies”,IEEE JOURNAL OF SOLID-STATE CIRCUITS, VOL. 41, NO. 11, 
NOVEMBER 2006.

* [4] 4.Akshay Bhaskar,“Design and Analysis of Low Power SRAM Cells”,International Conference on Innovations in 
Power and Advanced Computing Technologies [i-PACT2017].

* [5]Mukesh Kumar,Jagpal Singh Ubhi ,“Performance Evaluation of 6T, 7T & 8T SRAM at 180 nm Technology” ,8th 
ICCCNT 2017 July 3 - 5, 2017, IIT Delhi, Delhi, India.


