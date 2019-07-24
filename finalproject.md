# Final Project Proposal
This page will function as the home for the component parts of my final project proposal as I work toward ultimately completing it.

## Part #1
The following passes constitute the first part of my final project proposal.

### Project Outline and Overview
My final project for this class is connected to subject matter that I'm currently working on at my day job. One of my colleagues and I are the co-chairs of a collection of policy staffers in multiple offices that we've come to dub the Vacant, Abandoned, and Distressed Land Administration and Direct Services Policy Working Group, or the VLADS Policy Working Group for short. The goal our work thus far has been to partner with both internal and external stakeholders to offer hollistic operational and fiscal policy improvements that would better address vacant, abandoned, and distressed (VAD) land that's held by the City of Pittsburgh. For the purposes of my final project, I intend to hone in on vacant, publicly-owned land to illustrate the negative effects that City-owned vacant can produce, as well as touch on the need to allocate additional funding to certify this government-provided direct service as a greater priority for residents.

### The Data
I intend to use Allegheny County's [property assessment data](https://data.wprdc.org/dataset/2b3df818-601e-4f06-b150-643557229491/resource/f2b8d575-e256-4718-94ad-1e12239ddb92/download/assessments.csv), as updated for June 2019, pulled from the [Western Pennsylvania Regional Data Center](http://www.wprdc.org/).

Because this dataset is incredibly large, the subset that I'll use has been narrowed down based on the following filtering criteria:

| County Building Value | Local Building Value | Sale Price | Use Description                                                           | Tax Description | Property City       |
|-----------------------|----------------------|------------|---------------------------------------------------------------------------|-----------------|---------------------|
| 0                     | 0                    | 0          | Municipal Government,  Municipal Improvement, or  Municipal Urban Renewal | Exempt          | City of  Pittsburgh |
