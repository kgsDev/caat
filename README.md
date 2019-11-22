# CAAT
**Developed by**
Jason Dortch
Jason.M.Dortch@uky.edu
Kentucky Geologic Survey, University of Kentucky, Kentucky

**Summary**
Cosmogenic Age Analysis Tool (CAAT) isolates skewness from chronology datasets by separating Gaussians from probability density to estimate even age.  

**Installation**
The CAAT application was develop in the MATLAB environment and is compiled for standalone application without the need to purchasing MATLAB. If you do not have a copy of MATLAB, a prompt will appear to download MATLAB Runtime, which is ~1GB in size. A prompt about installing an application from an unknown publisher will likely appear. You must click yes to continue with installation. We recommend installing this application into a folder on your desktop or in your project folder. This is due to data table save function, which writes to the installation folder. Installing CAAT in a System32 folder will block write permissions and you will be unable to save your results.

**Description**
CAAT was develop in the MATLAB environment to isolate skewness from cosmogenic and cosmogenically calibrated Schmidt hammer exposure ages. It utilized the ksdensity function to calculate a probability density estimate from chronology data and the nlinfit function to isolate Gaussians based on a Monte Carlo approach.

**What you need:**
.txt file with four columns:
- Column 1 = moraine name
- Column 2 = age
- Column 3 = internal uncertainty
- Column 4 = external uncertainty

**Options:**
There are three bandwidth choices on the selection knob:

- **Mean** – the average uncertainty from column 2. Good to get an overview of your data.

- **Std** – A common bandwidth estimator which is the standard deviation of ages (column 1) X number of ages to the -1/5 power. Bandwidth can be too wide for vary scattered datasets. Works well with low sample numbers.

- **MAD** – a custom narrow bandwidth estimator that does a better job of de-weighting outliers and extreme scatter. It is the mean absolute deviation of ages (column 1) divided by two, X number of ages to the -1/5 power. Bandwidth can be too narrow for tightly clustered datasets.  Works well with high sample numbers.

- **Select preferred Gaussian number** – Identify the Gauss that best fits you event from the plot or data table and enter the gauss number in the box and hit enter. This will highlight all of the ages that fall within two sigma of that Gauss peak.

- **Save Table Results** – This button saves the model fitment data and the Gaussian data as .csv files.

- **Save Main plot** – use the file drop down menu on the plot to save it as your preferred file type. It is strongly suggested that you stretch the figure vertically to the height of your screen as having four subplots compresses the vertical axis.

Stay safe and have fun!
____________________________________________________________________________________________________________________________________

**CAAT – Cosmogonic Age Analysis Tool**
**End-User Agreement** - Read in full before installing the CAAT application.

By installing or using CAAT and clicking next, you explicitly agree to all terms in this statement. If you do not agree, do not install or use the CAAT application and select cancel instead.

**License:** You are granted revocable, non-exclusive, non-transferable, limited license to download, install and use the CAAT application solely for non-commercial personal academic purposes strictly in accordance with the terms of this Agreement.

**Restrictions:** You agree not to, and will not permit others to: license, sell, rent, lease, assign, distribute, transmit, host, outsource, disclose or otherwise commercially exploit the CAAT application.

By installing CAAT, you waive any rights to hold the Authors, their employers, & their institutions liable for: damage to your equipment, misuse, or poor interpretations resulting from the installation or use of the CAAT application. This includes, but is not limited to, if you or your intuitions computer(s)/network(s) is corrupted, resets, dies, melts, explodes, catches fire, shorts out, acts weird or buggy, interferes with other programs/applications, disappears into the either, and/or kills your dreams, prevents you from obtaining an academic degree, or makes you so smart you can no longer relate to others and feel isolated/depressed.

We reserve the right to modify, suspend (temporarily or permanently), or otherwise modify CAAT and subsequent versions without any liability to you.
