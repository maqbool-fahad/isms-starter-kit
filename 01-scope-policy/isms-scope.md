# ISMS Scope Statement: Havelmetrics GmbH


## 1. What the ISMS covers
The ISMS covers the development, hosting and support of StoreSight,
Havelmetrics' cloud dashboard for retail customers. It includes:
- The Azure production and test environments that run StoreSight
- The Azure SQL database that stores customer sales data and user accounts
- Private GitHub repositories holding the product source code
- Microsoft 365 and Microsoft Entra ID, used for email, files and sign-in
- Company laptops and the 40 staff who use them

## 2. Locations
- The Berlin office in Kreuzberg, used two days a week
- Remote work locations, mainly employees' homes

## 3. Exclusions
- Customers' own IT systems, because Havelmetrics does not control them
- Marketing website (hosted by an external provider): excluded because it
  contains only public information and is separate from the StoreSight
  environment. Contact form submissions are forwarded to the customer
  support tool, which is in scope (see Section 4). Website admin accounts
  use separate credentials from company systems.

## 4. Interfaces and dependencies
- Suppliers: payment provider, customer support tool, backup service
- Customer sales data flows into StoreSight through secure connections e.g customers upload sales data through an encrypted API or file transfer
- Staff access Havelmetrics systems from company laptops and, for email, from personal phones

## 5. Review
The scope is reviewed once a year and whenever there is a major change,
such as a new product, office or cloud provider.  
