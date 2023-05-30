-------------------
GENERAL INFORMATION
-------------------


1. Title of Dataset 

    Municipal Recycling

2. Author Information

    Name: Wendy Dorantes
        Institution: University of Washington
        Email: wdora@uw.edu

3. Date of data collection

	Data was collected from the United States Environmental Protection Agency’s, 

	“U.S. State and Local Waste and Materials Characterization Reports" for 2014.

4. Geographic location of data collection (where was data collected?): 

	Solid waste data was collected in California, Maine, and Thurston County, Washington.


---------------------
DATA & FILE OVERVIEW
---------------------


1. File List
    A. Filename: README.txt
        Short description: This file, information around the total dataset.
    B. Filename: 2014_CA_Municipal-Recycling.csv
        Short description: This file is a CSV with the normalized dataset of the tons of solid waste 
	collected across the state of California studied. 
    C. Filename: 2014_ME_Municipal-Recycling.csv
        Short description: This file is a CSV with the normalized dataset of the tons of solid waste 
	collected across the state of Maine studied. 
    D. Filename: 2014_WA_Municipal-Recycling.csv
        Short description: This file is a CSV with the normalized dataset of the tons of solid waste 
	collected across the state of Thurston County, Washington studied.

2. File Naming Convention
	
	 File names will follow a naming convention with year of the data first, followed by the abbreviation of the 
	state and finally ending it with "municipal_recycling".
    
-------------------------
DATA-SPECIFIC INFORMATION 
--------------------------


1. Data Structure & Normalization:
	Data was normalized by focusing on the itemized listing of solid waste collected and identifying which
	material subtypes were recyclable according to the guidlelines in which municipality the waste was collected.
	In the California dataset I looked at the 2014 data given recycling percentage by dividing the tons of recyclable
	waste collected by the total waste collectd in 2014 and calculating that percentage. For the Thurston County, Washington
	data the tons for the individual material subtypes were calculated by multiplying the precentage given by the complete tons 
	collected. These totals of recyclable waste collected and the percentage of recycled materials wsa given in the totals 
	at the bottom of each respective chart. 

	The data for Maine was normalized by calculating the the percentages of each material given. However, I was unable to index
	the material into subtypes. In addition, it was difficult to give a recycling percentage without relying on the vocabulary 
	already in the dataset. Maine divided the waste collected into two sections known as CDD = Construction/Demolition Debris
	and MSW = Municipal Solid Waste. Both these data sets are presented in the Maine page and have their own recycling rate which is later 
	combined in the totals section. 


2. Variable List
	A. Variable:Material
		Variable Name: Material of Waste
		Measurement Unit:String
		Allowed Values:Word phrase of any disposable material
		Description: The general category that the solid waste falls into

	B. Variable:Material_Subtype
		Variable Name:Material Subtype
		Measurement Unit:String
		Allowed Values:Word phrase of any disposable material
		Description: The specific items that the solid waste fall into

	C. Variable:Recyclable
		Variable Name:Recyclable 
		Measurement Unit:String
		Allowed Values:“Y”, “N”
		Description: Whether a material is recyclable in the municipality it is 
				collected in. "Y" meaning yes and "N"meaning no. 

	D. Variable:Percent
		Variable Name:Percentage of Solid Waste
		Measurement Unit:Percentage
		Allowed Values:0.0% to 100.0%
		Description: The percentage that the solid waste items makeup in the total amount collected

	E. Variable:Tons
		Variable Name:Tons of Solid Waste
		Measurement Unit:Integer
		Allowed Values:All real numbers
		Description: The tons in pounds collected of the solid waste

	