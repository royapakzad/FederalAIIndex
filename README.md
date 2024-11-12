# FederalAIIndex
The code and dataset used for the project The U.S. Responsible AI Procurement Index (2023)

We utilized USAspending.gov, an open data platform that provides federal procurement data across U.S. government agencies. We applied the keywords “artificial intelligence” and “machine learning” to capture procurement records that mentioned these terms in the contract descriptions. The search was limited to fiscal years 2023 and 2024 to align with the researcher’s fellowship timeline at UVA and to capture recent data relevant to Executive Order (EO) 13960 (2020), which emphasizes the acquisition of trustworthy AI technologies and underscores the importance of transparency and accountability in AI procurement within public-private partnerships.
To focus on relevant contracts, we filtered our search to include only “Contract” and “IDV Contract” award types. After narrowing the results by agency, we downloaded the data in CSV format for further processing.

Our data cleaning process used a Python script to extract only the necessary columns from the dataset, including contract details such as:
Basic Contract Info: ‘contract_transaction_unique_key,’ ‘awarding_agency_name,’ ‘recipient_name,’ ‘transaction_description,’ ‘award_type’
Financial and Timeline Information: ‘current_total_value_of_award,’ ‘period_of_performance_start_date,’ ‘period_of_performance_potential_end_date’
Compliance and Standards: ‘clinger_cohen_act_planning_code,’ ‘labor_standards,’ ‘performance_based_service_acquisition’
Diversity Indicators: ‘minority_owned_business,’ ‘woman_owned_business,’ and specific diversity attributes.
Competitiveness: ‘number_of_offers_received,’ ‘extent_competed,’ ‘solicitation_procedures,’ and ‘fair_opportunity_limited_sources,’ to assess the level of competition and exclusivity in AI contract procurement

Technology Type (NAICS Codes): ‘naics_description’ and ‘product_or_service_code_description,’ to identify the specific type of technology and services.
With the cleaned data, we developed additional Python scripts to answer each project indicator. These scripts facilitated the analysis of procurement practices, compliance with standards, and transparency across agencies, providing critical insights for each indicator.

