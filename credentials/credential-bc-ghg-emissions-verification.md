# BC GHG Emissions Report Verification Statement Credential

## Introduction
This document articulates the credential for the Emissions Report Verification Statement required for reporting GHG Emissions in British Columbia as per the Greenhouse Gas Industrial Reporting and Control Act, GREENHOUSE GAS EMISSION REPORTING REGULATION. When large emitters of CO2 report annual emissions to BC Climate Action Secreteriate, an Emissions Report Verification Statement must be provided as part of the reporting requirements.

B.C. Regulation 249/2015: https://www.bclaws.gov.bc.ca/civix/document/id/complete/statreg/249_2015
This regulation sets out reporting requirements that are developed in accordance with various standard setting bodies. Section 33 specifically references the International Accreditation Forum (IAF). Other sections within the regulation also refer to provisions being drafted in accordance with the International Standards Organization (ISO), the Western Climate Institute (WCI), the Canadian Standards Association (CSA) and the National Bureau of Standards (NBS). 

Current guidelines for reporting are described here: https://www2.gov.bc.ca/gov/content/environment/climate-change/industry/reporting/verify

This governance document has been developed in accordance with the ToIP’s Governance Metamodel Specification created by the Governance Stack Working Group (GSWG) as the template for this framework.

## Terminology and Notation

[Glossary - General Trust Over IP Terms](https://trustoverip.github.io/toip/glossary)

## Localization

1.	The standard language for this governing framework is American English.
 
## Governing Authority

BC Climate Action Secreteriat is the governing authority and party legally responsible for developing, maintaining and implementing the Governance Framework.
The contact for petitioners and relying parties of this GF is:
* 	Name ___________
* 	Title ____________
* 	Organization ___________
* 	Email ____________

## Purpose

The Verification Statement credential must be issued by a third-party verification body. The structure for the credential contains all information needed to fulfil this Verification Statement. These systems and governance will allow a more trustworthy ecosystem. This will be built under this governance framework. The purpose of this governance framework to outline all rules associated with governance, issuance, verification, and revocation of this Verification Statement credential.  

## Scope

The GF only covers the Verification Statement Credential

## Schema Definition

This schema definition follows the AnonCreds specification (https://anoncreds-wg.github.io/anoncreds-spec/)

Attribute | Format | Rules | Notes
--- | --- | --- | ---
verification_body_name | String | Not NULL | Regulation s.33(2)(a)	[Verification Body name.  Include full legal company name. Trade name may be referenced in parentheses if applicable.]
verification_body_address | String | Not NULL | Regulation s.33(2)(a) 	[Business Address]
accreditation | String | Not NULL | Regulation s.33(2)(h) 	[Name of member of the International Accreditation Forum (IAF) and associated identification number]
accreditation_status | String | Not NULL | Regulation s.33(2)(h) 	[Affirm accreditation status with the IAF is in good standing.]
lead_verifier_name | String | Not NULL | Regulation s.33(2)(b) 	[Lead Verifier’s name]
lead_verifier_email | String | Not NULL | Regulation s.33(2)(b) 	[Lead Verifier’s business email]
lead_verifier_phone | String | Not NULL | Regulation s.33(2)(b) 	[Lead Verifier’s telephone]
independent_peer_reviewer_name | String | Not NULL | Regulation s.33(2)(l) 	[Peer Reviewer’s name]
independent_peer_reviewer_email | String | Not NULL | Regulation s.33(2)(l) 	[Peer Reviewer’s business email]
independent_peer_reviewer_phone | String | Not NULL | Regulation s.33(2)(l) 	[Peer Reviewer’s telephone]
reporting_operation | String | Not NULL | Regulation s.33(2)(d)	[Legal name of the Reporting Operation ]
name_of_facility | String | Not NULL | Regulation s.33(2)(d)	[For Single Facility Operations the name of the Facility.  Include N/A if not applicable.]
facility_type | String | Not NULL | [Single Facility Operation, Linear Facilities Operation, or Electricity Import Operation] 
facility_address | String | Not NULL | Regulation s.33(2)(d)	[For Single Facility Operations, the geographic coordinates and street address of the Facility.  Include N/A if not applicable.]
facility_longitude | String | Not NULL | Regulation s.33(2)(d)	[For Single Facility Operations, the geographic coordinates and street address of the Facility.  Include N/A if not applicable.]
facility_latitude | String | Not NULL | Regulation s.33(2)(d)	[For Single Facility Operations, the geographic coordinates and street address of the Facility.  Include N/A if not applicable.]
total_emissions | String | Not NULL | Total Emissions Attributable to the Reporting Operation during the Reporting Period. 	[#] tonnes CO2e
total_emissions_not_reporting_only | String | Not NULL | Total Emissions that are not Reporting-Only Emissions Attributable to the Reporting Operation during the Reporting Period.	[#] tonnes CO2e
total emissions_reporting_only | String | Not NULL | Total Reporting-Only Emissions Attributable to the Reporting Operation during the Reporting Period.	[#] tonnes CO2e
total_co2_from_nonbiomass| String | Not NULL | Total amount of carbon dioxide from non-Biomass that is Attributable to the Reporting Operation during the Reporting Period.	[#] tonnes CO2
total_co2_from_nonbiomass_not_schedule_c | String | Not NULL | Total amount of carbon dioxide from Biomass not listed in Schedule C of the Regulation that is Attributable to the Reporting Operation during the Reporting Period:	[#] tonnes CO2
total_co2_from_nonbiomass_in_schedule_c| String | Not NULL | Total amount of carbon dioxide from Biomass listed in Schedule C of the Regulation Attributable to the Reporting Operation during the Reporting Period:	[#] tonnes CO2

<!---
BCGHG ID | String | Not NULL | Regulation s.33(2)(d)	[Number provided by the Director established under the Act. For inquiries contact GHGRegulator@gov.bc.ca]
Operator | String | Not NULL | Regulation s.33(2)(d)	[Legal name of Operator and head office mailing address.  If an Operator is an extraprovincial company with a head office outside British Columbia, provide the mailing address for the attorney.]
Operation Representative | String | Not NULL | Regulation s.33(2)(d)	[Name, Title, Business email and telephone for the Operation Representative.]
Person Primarily Responsible for Preparing and Submitting the Emission Report | String | Not NULL | Regulation s.33(2)(d)	[Name, Title, Business email, telephone and mailing address of the person primarily responsible for preparing and submitting the Emission Report.]
--->

## Credential Implementation
Ledger | SCHEMA DEF | CRED DEF | Notes	
--- | --- | --- | ---
BCovrin Test | ADCssx1nPW6FQwNHTFTRNW:2:BC_GHG_Emissions_Report_Verification_Statement:1.0 | --- | ---

