# Probe-matching
Associate the probe points to the correct road (link), Derive the slope from the probe points and Compare it to the surveyed slope in links file when possible

This homework has been achieved using Python 2.7 and the following libraries:
•	Math
•	Csv
•	Copy
•	Threading (if using multithreading which has issues)
•	Multiprocessing (if using multithreading which has issues)

Below is the list of filenames with descriptions

File	Description
math_functions.py	Helper function for math operations
parser_file.py	Helper function for parsing files
probe_matching.py	Map matching process
derive_slope.py	Slope Computation
probe_matching_multiThread.py	(Alternative/Additional) multithread map matching for cloud


To run the probe_matching.py and derive_slope.py programs you will have to indicate the following paths in the files:

File	Line	Path for the file
Probe_matching.py	101	Partition6467LinkData.csv
Probe_matching.py	102	Partition6467ProbePoints.csv
Probe_matching.py	103	Partition6467MatchedPoints.csv
Derive_slope.py	87	Partition6467MatchedPoints.csv
Derive_slope.py	27	SlopeComparison.csv
Derive_slope.py	88	Partition6467LinkData.csv


Then launch the python file corresponding to the task you want to perform:
•	Probe_matching.py if you want to match probe points and generation Partition6467MatchedPoints.csv file. 
•	Derive_slope.py if you want to calculate the slope for links and compare it to the surveyed file.

Note: 
1.	You have to run probe_matching.py first to compute the output file and be able to derive slope for a given link. Indeed, derive_slope.py requires data such as the link reference to compare the slope with the surveyed slope. 

2.	The total map matching process was executed for 1000 records only due to hardware limitations and high runtime.

