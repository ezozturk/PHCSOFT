# PHCSOFT

The PHCSOFT is a new scientific software encoded in the GNU C/C++ platform for the determination and visualization of physical height changes using GRACE-based GGMs.

In the computation file, firstly the PHCSOFT program should be compiled with this command:

g++ PHCSOFT.c -o PHCSOFT

Afterwards, the program can be run with this command:

./PHCSOFT -N60 -P75/25 -Fliste_CSR.txt -SSLR_C20.txt -LLLNs.txt

-N: the degree of harmonic coefficients that will be used in the computation can be selected,
-P: geodetic latitude/longitude of the computation point
-F: the data of SDS centers (options: CSR, GFZ or JPL) can be chosen that will be used in the computation
-S: the second d/o spherical harmonic coefficient C20 can be replaced by any other data (in the software, SLR_C20.txt includes Satellite Laser Ranging (SLR) data)
-L: For the estimation of the Earth’s surface displacements, the load Love numbers (LLNs.txt) calculated from the PREM can be employed.

In the plot file, fig1.bash (ΔN), fig2.bash (Δh) and fig3.bash (ΔH) can also be used to plot the time series.
