# MedElite Facility Assessment Report Generator
Edita Cosovic
Brown University PLME Program


This project was developed as part of the MedElite technical case study.

The application allows users to search for a skilled nursing facility using a CMS Certification Number (CCN), retrieve public CMS Provider Data, supplement the record with MedElite operational inputs, and generate downloadable facility assessment reports.

## Features

* Dynamic CCN lookup using the CMS Provider Data API
* Facility name override
* Location and certified bed count retrieval from CMS
* Manual operational inputs:

  * EMR
  * Current Census
  * Patient Type
  * Previous Coverage from MedElite
  * Previous Provider Performance
  * Medical Coverage
  * MedElite History
* CMS ratings:
  * Overall Rating
  * Health Inspection Rating
  * Staffing Rating
  * Quality Rating
* Occupancy calculation
* PDF report export
* Word (.docx) report export
* Clickable Medicare Care Compare source link
* Error handling for invalid or missing CCNs

## Technology Stack

* Python
* Flask
* ReportLab
* python-docx
* CMS Provider Data API

## Assumptions

* Occupancy is calculated as Current Census divided by Certified Beds.
* Blank manual fields are displayed as "Not Provided."
* The INFINITE branding remains fixed and is not replaced by facility names.
* Hospitalization and Emergency Department metrics were identified as optional bonus functionality and were not implemented.

## Running the Application

Install dependencies:

pip install -r requirements.txt

Run the application:

python main.py

Open in your browser:

http://localhost:8000

## Closing Note

Thank you for your time and consideration. I enjoyed putting this project together and learning more about the facility evaluation process, and I hope to be able to join the team this summer!
