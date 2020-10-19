# Data-Science-for-Space-Resaerch

#Space data Provider :

National Aeronautics and Space Administration is an independent agency(NASA),
-------------------
European Space Agency (ESA),
----------------------------
Canadian Space Agency(CSA), 
--------------------------
Japan Aerospace Exploration Agency (JAXA),....
---------------------------------------------------------------------------------------
Applications: Resaerch & Development ;Space exploration , Solar System, Earth Science, Public Health Environmental Science,Agriculture, Climate Change, natural Disasters,....................
-----------------------------------------------------------------------------------------------------------------------------------------------------
========================================
For better understanding:

(*)https://www.kaggle.com/sohelranaccselab/top-100-hubble-telescope-imagesvisualiaztion
----------
(*)https://www.researchgate.net/profile/Sohel_Rana5/publications
---------------
(*)https://www.researchgate.net/publication/343219641_SPACE_Weather_Impacts_on_Earth_Climate_A_case_Study_With_Remote_Sensing_Data
--------------------------------------------------------------------------------------------





It’s been a year since I started working in the data science industry. Coming from an aerospace engineering background, it’s only natural that I’d look for ways of applying AI, more specifically machine learning to space technology.

Historically, machine learning algorithms have been used in 

health monitoring of spacecraft, autonomous navigation, intelligent control systems and intelligent object detection for path navigation.
--------------------------------

Here, two approaches aiding in predictive analysis will be discussed. The first is the model-driven approach, which consists of a mathematical model for each subsystem of a spacecraft to correct the system to always adhere to the norm of that model.
The second approach is to collect data about the environment and the internals of the spacecraft in order to actively optimise functioning using machine learning models that best guess the situation. This is the data-driven approach, it proves to be more adaptable.
-----------------------------------------
1. Health Monitoring of Spacecraft
===============================================
In a spacecraft, there can be 1000+ monitored telemetry variables, that on-earth engineers analyse to diagnose abnormalities. An alternative data-driven approach has been suggested for anomaly detection by Takehisa Yairi and collaborators (Yairi et al.). The process takes into account five characteristics of telemetry data: High dimensionality, multimodality, heterogeneity, temporal dependence, missing data and trivial outliers. After the telemetry variables are normalised, they are used to create an integrated model called a mixture of probabilistic principal components analysers can categorical distributions (MPPCACD). Yairi et al. tested the model on telemetry data from the SDS-4, a demonstration satellite used by JAXA. A total of 89 continuous and 365 status variables were modelled. The performance of MPPCACD was compared to state of the art anomaly detection algorithms such as one-class support vector machine (OCSVM) and support vector data description (SVDD). The three algorithms function by producing an anomaly score graph, in which anomalies are denoted by graph spikes. In the graph out of MPPCACD, it was noted that in normal systems the anomaly scores are typically low (0–10) whereas anomalies are easily identifiable with scores of 100–200. As OCSVM and SVDD are general purpose method, the anomaly scores were erratic even in normal system operation making it difficult to distinguish anomalies.
-----------------------------------
2. Autonomous Navigation
=========================
A rover on Mars solely controlled by a team of engineers can only be given instructions to move every 20mins. This is the communication delay between Earth and Mars. Suppose only 5 movement commands can be sent every 20mins, that’s a total of 360 commands in a day. A rover equipped with autonomous navigation capability could make ≥ 5 decisions per min if not per second. It is now limited by the speed of its computer rather than the communication delay.
An artificial neural network (ANN) inspired model for satellite navigation is proposed by Mathew C. Wilkinson & Andrew J. Meade. Sequential Function Approximation (SFA) is used to develop an ANN that learns the effect of an engine burn through the variation of its magnitude and direction of burn on the flight path of the spacecraft. The result is compared to the desired state, the subsequent error parameter is used to constantly tweak the neuron parameters. SFA effectively trains its own neuron arrangement through an iterative process of observing the neuron parameter change’s effect on the error parameter. This approach was proven to more computationally efficient than computing dynamics equation or creating a neural map at once.
--------------------------------------------
-------------------------------------------------
3. Feature detection for planetary exploration
===============================================

The geographical features of the surface of a planet tell us about its geological makeup and its historical significance. The geographical analysis of nearby planets is enabled by on-ground rovers sending back images to earth. This can constitute a large volume of redundant data. This process could be a lot more efficient if the rover had an onboard mechanism to analyse features and classify images in order of significance, following which it can decide the best next action.
Burl, M. C., & Wetzler, P. G.evaluate the performance of a few supervised machine learning algorithms such as support vector machine (SVM) and continuously scaled template models (CSTM) to detect craters. The trained algorithms are tested with the Viking Orbiter images of Mars. The SVM approach was found to be the most effective, being as accurate as humans classifying the photos. The authors suggest a novel implementation of SVM using fast fourier transforms and overlap-and-add technique which reduces the memory usage to 5% of the images size. This allows the algorithm to be run on memory constrained systems such as a spacecraft.
------------------------------------------------------------
