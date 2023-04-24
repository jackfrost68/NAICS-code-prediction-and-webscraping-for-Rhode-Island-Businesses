# NTerprisers-Python-Project


<ins>*Problem 1: Generate a comprehensive list of private manufacturing companies</ins>*

The objective of this project was to identify private manufacturing companies registered in the states of Rhode Island and Massachusetts, and to extract their company names, addresses, and any available North American Industry Classification System (NAICS) codes.

To accomplish this, we utilized the Secretary of State websites for both states, which provided us with the necessary information. However, we filtered the companies to only include private manufacturing companies by matching the NAICS code to codes starting with 31, 32, or 33. For companies without a NAICS code or with a null or 999999 code, we automated web scraping of the respective SOS website for key indicators for NAICS.

After completing the above steps, we exported the final list of private manufacturing companies in the specified states with their assigned NAICS codes. This project was successful in achieving its objective of identifying private manufacturing companies in Rhode Island and providing relevant information for these companies.

<ins>*Challenges</ins>*
1. Inconsistent web scraping functionality on the Massachusetts SOS website leading to slow performance and frequent timeouts.

<ins>*Problem 2: Verify list of companies</ins>*

After retrieving the list of manufacturing companies located in Rhode Island and Massachusetts, we are conducting verification of each company's name using Neeva.com and Google Search API.
We are conducting web scraping of each entity name and attempting to locate the keyword "manufacturing" through this process.

The verification process of identifying manufacturing companies through web scraping using Google API and Neeva.com revealed varying levels of accuracy and error rates. The Google API resulted in an accuracy rate of 36.3% and an error rate of 63.6%, while Neeva.com yielded an accuracy rate of 66% and an error rate of 34%.

<ins>*Challenges</ins>*
1. Occasional 405 errors encountered while using  Neeva and Google search APIs preventing us from retrieving all desired values in a single query.
2. Large volume of data to be processed leading to lengthy processing time.


<ins>*Key Achievements</ins>*

1. Successful retrieval of the list of manufacturing companies in Rhode Island from the SOS website using web scraping.
2. Got an official list of 100 businesses from the Massachusetts Secretary of State office. 
3. A cache was implemented which reduced the retrieval time from 4 hours to 2 minutes.
4. 405 error during the web scraping process was managed effectively by creating the request in chunks.
5. The project's accuracy was verified through both Google API and Neeva.com verifying the integrity of the data gathered.
