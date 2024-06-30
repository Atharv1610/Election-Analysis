# Election-Analysis


This project involves extracting, analyzing, and organizing statewise election results data from the Election Commission of India (ECI) website.
The goal is to compile detailed insights into parliamentary constituency outcomes across various states, focusing on party-wise performance, winning candidates, and key electoral statistics. The information is organized into envelopes by state and party, working with complete investigation and reportage on political decision patterns and political elements.


## Table of Contents

- [Installation](#installation)
- [Data Extraction](#data-extraction)
- [Organizing CSV Files by State](#organizing-csv-files-by-state)
- [Training Procedure](#training-procedure)
- [Training Results](#training-results)
- [Applications](#applications)
- [Contributing](#contributing)
- [License](#license)


## Installation

1. Clone the repository:

   ```bash
   https://github.com/Atharv1610/Election-Analysis.git
   cd Election-Analysis
	```
2. Install the required Python packages:

   ```bash
   pip install -r requirements.txt
   ```

## Data Extraction
The Election-Analysis project begins by scraping comprehensive statewise election results data from the Election Commission of India (ECI) website. Using Python's requests and BeautifulSoup libraries, URLs are parsed to access detailed parliamentary constituency outcomes.
 ```bash
import requests
from bs4 import BeautifulSoup
import os

url = 'https://results.eci.gov.in/PcResultGenJune2024/index.htm'

response = requests.get(url)
soup = BeautifulSoup(response.content, 'html.parser')
   ```


## Organizing CSV Files by State
The election data collected from the Election Commission of India (ECI) website is meticulously organized into a structured folder hierarchy. Each state registry inside the 'state' envelope contains subfolders addressing individual ideological groups. Inside each party organizer, CSV documents exemplify itemized parliamentary electorate results, including characteristics, for example, seat number, parliament supporters, winning applicant, all out votes, and edge. This systematic arrangement ensures efficient data retrieval and comprehensive analysis of statewise election outcomes, facilitating detailed insights into electoral trends and political dynamics across India.
