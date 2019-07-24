# Final Project Proposal
This page will function as the home for the component parts of my final project proposal as I work toward ultimately completing it.

## Part #1
The following passes constitute the first part of my final project proposal.

### Project Outline and Overview
My final project for this class is connected to subject matter that I'm currently working on at my day job. One of my colleagues and I are the co-chairs of a collection of policy staffers in multiple offices that we've come to dub the Vacant, Abandoned, and Distressed Land Administration and Direct Services Policy Working Group, or the VLADS Policy Working Group for short. The goal our work thus far has been to partner with both internal and external stakeholders to offer hollistic operational and fiscal policy improvements that would better address vacant, abandoned, and distressed (VAD) land that's held by the City of Pittsburgh. For the purposes of my final project, I intend to hone in on vacant, publicly-owned land to illustrate the negative effects that City-owned vacant can produce, as well as touch on the need to allocate additional funding to certify this government-provided direct service as a greater priority for residents.

### The Data

#### Allegheny County Property Assessments Parcel Data
I intend to use Allegheny County's [property assessment data](https://data.wprdc.org/dataset/2b3df818-601e-4f06-b150-643557229491/resource/f2b8d575-e256-4718-94ad-1e12239ddb92/download/assessments.csv), as updated for June 2019, pulled from the [Western Pennsylvania Regional Data Center (WPRDC)](http://www.wprdc.org/).

Because this dataset is incredibly large, the subset that I'll use has been narrowed down based on the following filtering criteria:

| County Building Value | Local Building Value | Sale Price | Use Description                                                           | Tax Description | Property City       |
|-----------------------|----------------------|------------|---------------------------------------------------------------------------|-----------------|---------------------|
| 0                     | 0                    | 0          | Municipal Government,  Municipal Improvement, or  Municipal Urban Renewal | Exempt          | City of  Pittsburgh |

In doing so, I'm able to ascertain that propertyies assessed at a County-level taxable value of $0, a City-level taxable value of $0, and a sale price of $0 that's documented as in use for only municipal government purposes, holds a tax-exempt status, and is located within the geographical boundaries of the City of Pittsburgh are vacant, City-owned parcels. Thus, I'm able to reduce this dataset from close to 580,000 entries to 7,000. This data subset, filtered-down using my selected criteria, is [available here](https://data.wprdc.org/dataset/property-assessments/resource/f2b8d575-e256-4718-94ad-1e12239ddb92?filters=SALEPRICE%3A0%7CPROPERTYCITY%3APITTSBURGH%7CTAXDESC%3A10+-+Exempt%7CUSEDESC%3AMUNICIPAL+GOVERNMENT%7CUSEDESC%3AMUNICIPAL+IMPROVEMENT%7CUSEDESC%3AMUNICIPAL+URBAN+RENEWAL%7CCOUNTYBUILDING%3A0%7CLOCALBUILDING%3A0).


#### Citywide Revenues and Expenses
The City of Pittsburgh has published [data through the WPRDC that documents its revenues and expenses](https://data.wprdc.org/datastore/dump/f61f6e8c-7b93-4df3-9935-4937899901c7) — as allocated and subsequently spent down in accordance with its yearly Operating Budget — from FY 2012 onward. As noted on the [WPRDC's page for this data](https://data.wprdc.org/dataset/city-revenues-and-expenses):

> City Revenues and Expenses from the Operating Budget from 2012 to Present, updated every night from the City's JD Edwards ledger.

However, I'm not interested in this entire dataset, so I'll narrow my search once again. I'm able to eliminate all entries in the dataset except for those related to the Department of Finance. Using "Three Taxing Bodies Trust Fund," also known as 3TB Trust Fund, as the value for the filter "Fund Description," I have access to all revenues and expenses associated with the specific fund that the City uses to finance the maintenance of the vacant property that it owns, [which can be viewed here](https://data.wprdc.org/dataset/city-revenues-and-expenses/resource/f61f6e8c-7b93-4df3-9935-4937899901c7?filters=department_name%3ADepartment+of+Finance%7Cfund_description%3ATREE+TAXING+BODIES).  

Due to issues with the WPRDC website, though, I elected to download that dataset as a .csv file and then use Microsoft Excel's built-in filtering tool to the data to only show me results for entries marked "Maintenance" or "Landscaping" for the criteria of "Object Account Description," which indicates to a user the activity that either produced revenue for the 3TB Trust Fund or required an expenditure. I'm also able to use a similar method to find "Administrative Fees" and "Legal Fees," but it's more difficult to associate those specifically with stewardship of vacant parcels. To validate my uncertainty, I'm able to cross-reference the "Object Account Descriptions" and the "Object Account Number" with the City's Operating Budget. For example, I used the [FY 2019 Operating Budget](https://apps.pittsburghpa.gov/redtail/images/4650_2019_Operating_Budget_as_amended.pdf) when working with this dataset in the aforementioned situation.