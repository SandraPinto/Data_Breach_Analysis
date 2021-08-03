# Analyzing Data Breaches with Python 
![data breach](https://user-images.githubusercontent.com/43500549/127944516-6f78013c-e1f5-439c-86ac-60376bb5e6da.JPG)

**PHASE I- PROJECT OVERVIEW**

Cybercrime is a growing problem and according to the latest Verizon Data Breach Investigations Report, North America alone accounts for 55% of total data breaches in the world which only 920 incidents were publicly disclosed in 2020 (2020 Data Breach Investigations Report). Recent events such as the SolarWinds (APT𑁋Trojan Horse), the Colonial Pipeline hack (Ransomware), and JBS Foods attacks have affected millions causing tremendous loss and revealed serious gaps in cyber defenses in both public and private organizations. 

For instance, companies such as Accenture are using Natural Language processing to unlock the value of Cyber data in user cases such as Insider Threat detection. According to the Ponemon Institute’s report, " the overall cost of insider threats is rising, with a 31% increase from $8.76 million in 2018 (Ponemon) to $11.45 million in 2020. In addition, the number of incidents has increased by a staggering 47% in just two years, from 3,200 in 2018 (Ponemon) to 4,716 in 2020.”(Ponemon Institute). 
 The purpose of this project is to close the gaps in properly labeling  and classifying observations against type of breach and industry to make better predictions and ideally prevent or better prepare for  future attacks, ultimately reducing potential damage. The ultimate objective of NLP is to read, decipher, understand, and make sense of the human languages in a manner that is valuable hence Cyber Security is highly composed of text. 
 
**Data Set**

For my capstone project, I’m using the data set Chronology of Data Breaches by the Privacy Rights Clearinghouse, a nonprofit organization that empowers individuals and advocates for positive change within the ever-changing privacy landscape. Most of the data was sourced from State Attorneys General and  the U.S. Department of Health and Human Services which is regularly updated. The units of analysis are the following: City, state, company, type of breach, type of industry, Description of incident, the date made public, the source, the year of breach, the number of total records, the URL, the latitude, and longitude, and etc. The Data Set is composed of 13 columns, 9015 rows, 4375 KB (4.375 MB), and contains both numerical and text data. 

**Type of Breach**

CARD𑁋Fraud Involving Debit and Credit Cards Not Via Hacking (skimming devices at point-of-service terminals, etc.)
HACK𑁋Hacked by an Outside Party or Infected by Malware
INSD𑁋Insider (employee, contractor or customer)
PHYS𑁋Physical (paper documents that are lost, discarded or stolen)
PORT𑁋Portable Device (lost, discarded or stolen laptop, PDA, smartphone, memory stick, CDs, hard drive, data tape, etc.)
STAT𑁋Stationary Computer Loss (lost, inappropriately accessed, discarded or stolen computer or server not designed for mobility)
DISC𑁋Unintended Disclosure Not Involving Hacking, Intentional Breach or Physical Loss (sensitive information posted publicly, mishandled or sent to the wrong party via publishing online, sending in an email, sending in a mailing or sending via fax) 
UNKN𑁋Unknown (not enough information about breach to know how exactly the information was exposed)

**Type of Business**

BSF𑁋Businesses (Financial and Insurance Services)
BSO𑁋Businesses (Other)
BSR𑁋Businesses (Retail/Merchant including Online Retail)
EDU𑁋Educational Institutions
GOV𑁋Government & Military
MED𑁋Healthcare, Medical Providers and Medical Insurance Services
NGO𑁋Nonprofits
UNKN𑁋Unknow

**Research Question & Implementation**

1.Accurately classify the types of breaches per industry.
2.Perform K-means in order to determine the optimal number of breach categories.
3.Conduct an NLP model to predict type of Breach based on Description of Incident (text).


**PHASE II- EDA & MODEL CONSTRUCTION**

I created a pie chart showing the percentage of data breaches per organization type in which shows that the type of organizanations which the most data breach incidents are MED (Healthcare, Medical Providers and Medical Insurance Services) and BSO(Businesses𑁋Other)
![image](https://user-images.githubusercontent.com/43500549/127945528-8e579d6a-0152-4c34-9156-bbdc132a1cfd.png)

I created a bar graph showing the total number of incidents per breach in which HACK (Hacked by an Outside Party or Infected by Malware) is the type of breach with the highest number of reported incidents per my dataset. 

![image](https://user-images.githubusercontent.com/43500549/127946579-ce080675-cb6d-477c-9bea-b7fee0165c1c.png)

The below pie chart shows the top 5 states with the most hacks:

![image](https://user-images.githubusercontent.com/43500549/127946982-6567b3ca-1c0b-4e03-ba79-41fa8b075bcd.png)


After cleaning and parsing my text data, I was able to create the below wordcloud showing the most frequently occuring words. 

![image](https://user-images.githubusercontent.com/43500549/127946805-188122f0-585e-42e9-af9c-43fae9fdf67a.png)



**Sources:**

*2020 Data Breach Investigations Report. (n.d.). Verizon Enterprise Solutions. Retrieved April 19, 2021, from https://enterprise.verizon.com/resources/reports/2020-data-breach-investigations-report.pdf
*Thompson, T. (n.d.). The Colonial Pipeline cyber attack and the SolarWinds hack were all but inevitable. Why national cyber defense is a “wicked” problem—Virginia Mercury. Retrieved June 14, 2021, from https://www.virginiamercury.com/2021/05/13/the-colonial-pipeline-cyber-attack-and-the-solarwinds-hack-were-all-but-inevitable-why-national-cyber-*defense-is-a-wicked-problem/ 
*James. (2019, October 7). Using NLP to Analyse Organisational trends in Data Breaches. Medium. https://medium.com/@jameskay_25745/using-nlp-to-analyse-organisational-trends-in-data-breaches-cc47053224f9
*Industry use case:  https://www.accenture.com/_acnmedia/PDF-106/Accenture-Unlocking-Value-Unstructured-Data.pdf 
*Dataset:
Data Breaches | Privacy Rights Clearinghouse. (n.d.). Retrieved June 14, 2021, from https://privacyrights.org/data-breaches

