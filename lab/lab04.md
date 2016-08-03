# lab04

## TITLE:
Measurement of Antenna Performance Parameters

## BACKGROUND:
As you have seen in the lectures, there are various types of antenna topologies. One group is a resonant type antenna. They operate well at a specific frequency (resonance frequency) and exhibit a relatively narrow bandwidth (on the order of few percent). Often one dimension of a resonant antenna is $$ \tfrac{\lambda}{2}$$. In [Lab 3](lab03.md), you designed and simulated a resonant antenna, i.e. microstrip patch antenna. In this experiment, you will investigate the half-wave dipole antenna which is the most fundamental resonant antenna topology. Half-wave dipoles are made out of wire cylinders or conductor traces on a printed circuit board (PCB) substrate. One arm of the dipole is connected to the signal trace and the other (or ground) path.

Radiation characteristics of any antenna are evaluated through a set of tests. The resonance frequency is found by measuring the reflection coefficient or $$S_{11}$$ by a Vector Network Analyzer (VNA). The radiation pattern of an antenna is measured at specialized test facilities such as an Antenna Range or an Anechoic Chamber. At these special facilities, the measurement environment isolates the antenna under test (AUT) from ambient RF signals and remove all the possible reflections from the surroundings in order to solely measure AUT’s radiation. Usually these specialized spaces for antenna measurement require a large space, or a shield room covered with special absorbing material. By using a transmitter and rotating a receiver shape of radiation pattern can be estimated.

The set- up, that is used in this experiment (DreamCatcher ME1300), with the aid of a software tool (RadPat) and an RF signal generator creates the radiation pattern of an antenna under test. This set-up has a transmitter (Tx) unit that is fed by the signal generator and a receiver (Rx) unit. The Rx unit sends the received signal to the computer to plot the radiation pattern. Two identical antennas are provided for this purpose each connected to the top of Rx or Tx posts (Note these posts are like antenna towers). The Rx post can be rotated and is controlled by RadPat software. Rotation of Rx post allows measuring the magnitude of the received signal at different angles. The angular steps can be specified on the user interface of RadPat software. This recording of the Rx signal versus angle is basically plotting the radiation pattern.

Different cut-planes of the radiation pattern can be created by changing the orientation of Rx/Tx antennas. Please refer to the Appendix to this lab handout which is documentation from the ME1300 manufacturer (DreamCatcher Company) to see pictures of the two possible orientations to be used for this measurement. Since we are working with dipoles, the two vertical and horizontal orientations of the antennas pertain to vertical and horizontal polarizations (linear polarization)

Remember from ELEN105 lecture discussions that the orientation of the Tx and RX antennas with respect to each other (or in a more accurate term polarization of the two antennas) is an important design factor in establishing a communication link.

## OBJECTIVE:
In this experiment, you will measure the resonance frequency, bandwidth, input impedance and radiation pattern of three printed dipole antennas. First you will use a Vector Network Analyzer to determine the resonance frequency, bandwidth, Zin and VSWR. Then, you will use the ME1300 set up to measure the radiation pattern of 3 dipole antennas.

## EQUIPMENT:
- Vector Network Analyzer
- Dream Catcher ME1300 training kit
- Signal Generator
- A pair of two identical printed dipole antennas operating at $$433\:\text{MHz}$$
- A pair of two identical printed dipole antennas operating at $$915\:\text{MHz}$$
- A pair of two identical printed dipole antennas operating at $$2.4\:\text{GHz}$$

## PRELAB:
The length of a half-wave dipole is approximately $$\tfrac{\lambda}{2}$$.
- Consider a dielectric constant of 1 and calculate the length of half-wave dipole antennas operating at $$433\:\text{MHz}$$, $$915\:\text{MHz}$$ and $$2.4\:\text{GHz}$$.

To create a printed dipole a dielectric substrate is used and conductor traces make the two dipole arms on the two side of the board. The dielectric constant of the substrate used in this lab is not known but its thickness is measured to be around 4.5.
- Use a ruler to measure the length of three printed antennas. Compare these numbers with what you calculated in question 1.
- Can you determine the value of $$\epsilon_\text{eff}$$ from what you found is questions 2 and 3?
- If a substrate with $$\epsilon_\text{r}$$ of 4.5 is used for making these antennas and the formula used for determining the εeff of a microstrip line is used for calculating $$\lambda$$, what do you find for the lengths of the 3 dipole antennas? Create a table comparing the answers of questions 1, 2 and 4.


## PART I:
MEASUREMENT OF RESONANCE FREQUENCY, BW, VSWR.

In this part, first, you verify the resonance frequencies of 3 different printed dipole antennas, i.e. $$433\:\text{MHz}$$, $$915\:\text{MHz}$$ and $$2.4\:\text{GHz}$$. For this, you will use a VNA and observe $$S_{11}$$. You need to calibrate the VNA (1-port Short Open Load Calibration) to the appropriate frequency range. Refer to Lab 2 procedure and follow the needed steps to calibrate the VNA. Then, you should also obtain VSWR and $$Z_\text{in}$$ plots.

### PROCEDURE:
- For 433 MHz and 915 MHz dipole antennas select the calibration frequency range of 300MHz to 1100MHz. Measure S11 for each dipole. Include the S11 plots of both antennas (in dB) in your report. To show the plots well, reduce the plot’s frequency range of plotting to what seems to be appropriate to show the bandwidth and resonance.
- What is the measured resonance frequency of each dipole antenna? This is the frequency at which you see the minimum S11.
- What is the 10 dB bandwidth for each dipole?
- For each antenna measure VSWR and Zin (both real and imaginary parts). Include VSWR and input impedance (Zin) plots in your report. Show Zin on a Smith Chart. What is the VSWR<2 bandwidth for each antenna?
- For the 2.4GHz dipole select the calibration range of 2GHz- 2.8GHz. Measure and plot the magnitude of S11 in dB.
- MeasureandplotVSWR.WhatistheVSWR<2bandwidth?
- Measure and plot the input impedance (both real and imaginary parts. Show Zin on a Smith Chart.


## PART II:
MEASUREMENT OF RADIATION PATTERN

The set-up for measuring the radiation pattern using ME1300 Rx and Tx units, Signal generator and RadPat software is shown in Figure 2 of the Appendix. This set-up is already connected, set and calibrated for you to measure radiation pattern of 2.4GHz dipole antenna.

To do this, you need to use an identical pair of AUTs and connect one to the Rx post and the other to Tx. Set the frequency range as follows;
- For 2.4GHz dipole from 2.3GHz to 2.5GHz

To measure $$E$$-plane cut of the radiation pattern of the dipole, these antennas should be placed horizontally (See Figure 3 in the Appendix).

To measure $$H$$-plane cut of the radiation pattern of the dipole, these antennas should be placed vertically (See Figure 4 in the Appendix).

To perform radiation pattern measurement we should place Rx antenna at the far field range distance from Tx antenna. One candidate formula given in the text book and also in the Appendices here is $$r_{ff}> \tfrac{2D^2}{\lambda}$$. Another one is $$R_{ff}>3\lambda$$. $$\lambda$$ is wavelength in free space.
 - Calculatethefarfieldrangeusingbothrff>2D2/λ.andRff>3λ.formulas.
- Place the antennas with horizontal orientation and conduct two sets of radiation pattern measurements while placing Rx and Tx antennas once at ( r = rff+ λ/2) and then at (r = Rff+ λ/2). For each measurement record the received power using the measurement sheet in Appendix A.
- 14. Using Matlab or any other function plotting software, create a rectangular plot of Normalized PR (dB) = PR (dBm) – max PR (dBm) versus angle for the two set of measurements in Step 13.
- When the antennas are at (r = Rff+ λ/2) distance, measure E-plane pattern and plot the normalized data recorded using the polar plot in RadPat.
- Now position the antennas vertically with the same (r = Rff+ λ/2) distance to measure H-plane pattern. Use the sheet in Appendix A to record the received power. Create the polar plot of H-plane pattern with RadPat and include it in your report.
- Do the E-plane and H-plane plots match what is expected from theory for radiation pattern of a dipole antenna? Verify this with your text book.
- What is the E-plane 3-dB beamwidth of the dipole antenna? What is its theoretical value?


## APPENDICES
ANTENNA PATTERN MEASUREMENT USING ME300

*Courtesy of Dream Catcher Company, the manufacturer of the ME1300 Antenna training kit*

### A. INTRODUCTION
An antenna radiation pattern is a representation of the field strength or power intensity versus the antenna orientation angle. For a receiving antenna, the antenna radiation pattern shows the received signal level at various directions (angles). Similarly, for a transmitting antenna, the antenna radiation pattern shows its field strength at various directions at a constant distance. The antenna radiation pattern of most antennas is valid when receiving and transmitting.

An antenna radiation pattern may consist of several lobes. Most of the power is concentrated in the main lobe. The 3-dB beamwidth is the angle between two points, which are $$3\:\text{dB}$$ lower than the main lobe maximum. Figure 1 illustrates the radiation pattern lobes together with different power points and beamwidths.

![fig01](lab04/lab04-fig01.png)
Figure 1 - Radiation Pattern Lobes

The antenna radiation pattern is usually shown in two planes. For a dipole antenna, its $$H$$-plane antenna radiation pattern will be plotted if both antennas are placed vertically, while its $$E$$-plane antenna radiation pattern will be plotted if both antennas are placed horizontally. The $$E$$-plane radiation pattern is defined as “the plane containing the electric field vector and the direction of maximum radiation”, and the $$H$$-plane radiation pattern is defined as “the plane containing the magnetic field vector and the direction of maximum radiation”.

Antenna radiation pattern measurement should take place in the far-field region. The distance between both antennas, $$r$$, must be large enough so that the antennas are in the far-field region where,

$$
r>\frac{2D^2}{\lambda}
$$
where $$\lambda$$ is wavelength and $$D$$ represents the largest dimension of the antenna under test (AUT)

In a confined space, the main sources of error in antenna measurement are due to reflection from nearby objects, walls, ceiling, and ground. To reduce the amount of reflection, the two antennas should be placed __(a)__ as far away as possible from any reflecting objects, and __(b)__ as close as possible to each other subject to the far-field criteria.

### B. ANTENNA RADIATION PATTERN MEASUREMENT

#### B.1 Using the Dipole Antenna
__NOTE__: To get the best accuracy, you should perform calibration before making any measurements on your RF detector. Please refer to Appendix C for the calibration procedure.

![fig02](lab04/lab04-fig02.png)
Figure 2 - Equipment Setup

- Set up the equipment as shown in Figure 2.
- 915 MHz λ/2 dipole antennas are used for the measurement. Mount the dipole antenna on the top connector of the fixed antenna holder on the transmitter module (TX). This is the transmitting antenna. Orientate the antenna for horizontal polarization and broadside to the other antenna-under-test (AUT).
- Use an RF coaxial cable to connect the RF OUT connector of an RF signal generator to the RF IN connector of the transmitter module (TX).
- Mount the other 915 MHz dipole antenna (AUT) on the top connector of the rotatable antenna holder on the receiver module (RX). This is the receiving antenna. Orientate the receiving antenna broadside to the transmitting antenna as shown in Figure 3 for horizontal polarization and maximum reception.

![fig03](lab04/lab04-fig03.png)
Figure 3 - Orientation of Receiving and Transmitting Antennas for Horizontal Polarization

1. Connect the __RF IN__ connector and __RF OUT__ connector on the receiver module (RX) using a coaxial cable (to send the signal back to the RF detector).
2. Adjust the distance between the antennas to $$50\:\text{cm}$$ and make sure that they are in the far-field region. Record the distance and the heights of the antennas in the corresponding record form as given in Appendix A.
3. Open the RadPat software and select the desired __PC ComPort__ under __Settings > ComPort__ tab.
4. Set __Baud Rate__ to __57600__ under __Settings > ComPort__ tab. Click the Instrument tab and unselect Enable Instrument. The RF detector will be activated when the Enable Instrument is unselected.
5. In the RF signal generator, set Frequency to 915 MHz. This is the frequency of the antenna-under-test (AUT).
6. Set Power Level to -10 dBm.
7. Click the Measurement tab and set Deg/Step to 10, 0-dB Ref: to –20 dBm, and Scale
to 15 dB/Div.
8. Click Connect to bring the rotator back to its home position.
9. After the homing operation, the window will return to the RadPat main interface. Click
Run at the menu bar to perform the Start, Pause, Stop, and Homing operations of the
rotator.
10. Click Run at the menu bar followed by Start to begin the antenna radiation pattern
plotting.
11. Observe the plotting and record the received signal strength at each step (e.g., 10°) in
the corresponding record form as given in Appendix A.
12. Determine the value of max PR, based on the radiation pattern plotting and calculate the
Normalized (dB) value for each step.
13. Using the polar chart in Appendix B, plot the antenna radiation pattern according to the
normalized data recorded. Compare the hand-plotted antenna radiation pattern with the one plotted using the RadPat software.

The orientation of the receiving and transmitting antennas for vertical polarization is shown in Figure 4.

![fig04](lab04/lab04-fig04.png)
Figure 4 – Orientation of Receiving and Transmitting Antennas for Vertical Polarization



