# Emission Factor Management in IBM Envizi

## 1. Objective
The objective of this article is to help understand how Envizi manages the Emission factors  

## 2. What are Emission Factors and why those are important

When Organization started their Sustainability journey, the very crucial thing is to start capturing the relevant  data with respect to their operations to estimate / calculate the emissions. The captured data should be cleaned, normalized and then used to calculate the organization emissions. So to calculate emissions, two types of input data is required. 

#### 1. Activity data
Activity data is a quantitative measure of a level of activity that results in GHG emissions. This is the data the organization captures from their operations / supply chain,etc.
Example :
- How many litres of fuel consumed, 
- How much electricity is consumed, 
- How many kilograms of material purchased

#### 2. Emission factor
An Emission factor is a factor that converts activity data into GHG emissions data.
Example :
- How much kg CO2 is emitted per litre of fuel consumed
- How much kg CO2 is emitted for one kwh power consumption 
- How much kg CO2 is emitted per kilograms of material produced

In other words, emission factors helps organizations to calculate the emissions or co2 equivalent of Greenhouse gases which are emitted because of the activities performed by their business. 

## 3. Who develops  the Emissions Factors ?

The Governments, environmental agencies, organizations, research institutes publishes the emission factors for numerous activity based data,  based on the scientific studies and experiments conducted considering various parameters, conditions, states , regions , etc

Below are the some of the well-known emission factor sets published by various organizations and countries. 

- ***International Energy Agency (IEA)*** publishes a comprehensive set of  Electricity and Heating emission factors annually covering most countries and regions in the world. Hence this emission factor set is leverage globally when the country or region specific emission factors are not available.  [more info](https://www.google.com/)

- ***Environmental Protection Agency (EPA)*** of United States, publishes emission factors for  electricity purchased from eGRID, mobile combustion, upstream and downstream transportation, business travel, product transport, and employee commuting.   [more info](https://www.google.com/)

- ***Department for the Environment, Food and Rural Affairs (DEFRA)*** and the UK Government publishes a comprehensive set of  GHG emission factors covering Scope 1, 2 and some Scope 3 emission sources. Mainly applies to UK, however company across Europe use this factor set.  [more info](https://www.google.com/)

- ***New Zealand Ministry for the Environment*** publishes GHG emission factors covering Scope 1, 2 and some Scope 3 emission sources.  [more info](https://www.google.com/)

- ***The Australian Government*** publishes GHG emission factors covering Scope 1, 2 data sources. [more info](https://www.google.com/)

- ***Eora’s MRIO (Multi-region input-output)*** provides spend-based emission factor set across 66 industry sectors, which is globally recognized.  [more info](https://www.google.com/)


## 4. What are the Supported Emissions Factors in Envizi ?

Envizi supports emissions calculation for all Scope 1, Scope 2 and Scope 3 activity data. Envizi maintains a emission factor library which contains all the publicly available emission factor sets as well as licensed factor sets, covering Scope 1, Scope 2 (both Location based and Market based) and Scope 3 (all categories supporting Spend-based / average data / supplier specific )

The managed emission factor sets includes the publicly available emission factors such as IEA, US eGRID, UK Defra, NGRES, Residual Mix Green-e, Residual Mix AIB, Eora66, USEEIO,NGRES + NGA, New Zealand Factor set, etc.  Below table provides the list of Manged Emission factors in Envizi as of date Nov 2023 with more details.  Please refer [Envizi knowledge base](https://knowledgebase.envizi.com/home/managed-emission-factors) for latest updates.
#### Factor Set
<table>
<tr>
        <th width="15%">Managed Factor Set</th>
        <th width="25%">Coverage </th>
        <th width="25%">Data types / Scopes </th>
        <th width="35%">Details </th>        
    </tr>
    <tr>
        <td>

[IEA](https://knowledgebase.envizi.com/home/managed-emission-factors-iea)
        </td>
        <td>
            <li>Applies Global
            </li>
            <li>Applies Majority of the countries where managed Emission factors are not available in Envizi
            </li>
            <li>
            Location based
           </li>
        </td>
        <td>
            <li>Scope 2: electricity and electricity green offset</li>
            <li>Scope 3: electricity</li>
        </td>
        <td>
            <li>Publisher: 
[The International Energy Agency](https://www.iea.org/data-and-statistics/data-sets) </li>
            <li>Licensed version</li>
            <li>Envizi has managed this factor set since 2013. </li>
            <li>Part of Envizi’s Default factor set</li>
            <li>Use only for in-house reporting, and must NOT be distributed or used outside of Envizi
            </li>
            <li>Review the factors using report - Emission and Energy Factors - PDF Version
            </li>
        </td>
    </tr>   
    <tr>
        <td>

[Eora66 - MRIO](https://knowledgebase.envizi.com/home/managed-emission-factors-eora-mrio-multi-region-in)
        </td>
        <td>
            <li>Applies to Global – 188 Countries</li>
            <li>Scope 3 </li>
        </td>
        <td>
            <li>Scope 3: Spend-based factor set covers 66 summary data types and relates to the US EEIO Summary classification</li>
        </td>
        <td>
        <li>
[Eora’s MRIO (Multi-region input-output)](https://worldmrio.com/)is a globally recognized spend-based emission factor set
</li>
    <li>Envizi managing this factor from June 2023</li>
    <li>IBM Envizi has modified Eora concordance tables to align with Summary categories provided by the US EPA providing coverage of 66 industries / commodities.</li>
        </td>
    </tr>   
    <tr>
<td>

[US eGRID - Electricity factors](https://knowledgebase.envizi.com/home/managed-emission-factors-us-egrid-electricity-fact)
        </td>
        <td>
            <li>US only (including Puerto Rico))
            </li>
            <li>
            location based
           </li>
        </td>
        <td>
            <li>Scope 2: electricity and electricity green offset</li>
            <li>Scope 3: electricity</li>            
        </td>
        <td>
            <li>Publisher: 
[US EPA (Environmental Protection Agency)](https://www.epa.gov/egrid) publishes eGRID database </li>
            <li>Envizi has managed this factor set since 2008 </li>                        
        </td>
    </tr>   
    <tr>
        <td>
[UK Defra](https://knowledgebase.envizi.com/home/managed-emission-factors-defra)
        </td>
        <td>
            <li>Applies to Europe for Scope 1  & Scope 2 - Location based            
           </li>
            <li>Global - Air travel and some other Scope 3 factors
            </li>
        </td>
        <td>
            <li>Scope 1: fossil fuels, biofuels, refrigerants, passenger and delivery vehicles (distance based)</li>
            <li>Scope 2: UK electricity, UK electricity for electric vehicles, heat and steam</li>
            <li>Scope 3: upstream and downstream emissions resulting from Scope 1 and 2 emission sources and… for more info refer factor page</li>
        </td>
        <td>
            <li>Publisher:
[UK Government and the Department for the Environment, Food and Rural Affairs (DEFRA)](https://www.gov.uk/government/collections/government-conversion-factors-for-company-reporting)</li>
            <li>Envizi has managed this factor set since 2009 </li>
            <li>Applies mainly to the United Kingdom but many organizations have chosen to apply this factor set across their European sites, particularly with emissions resulting from air travel.</li>
        </td>
    </tr>     
    <tr>
    <td>
[Residual Mix Emission Factors, Green-e](https://knowledgebase.envizi.com/home/managed-emission-factors-green-e-residual-mix)
        </td>
        <td>
            <li>Applies to US eGrid regions           
           </li>
            <li>Market-based
            </li>
        </td>
        <td>
            <li>Scope 2: Market-based electricity
        </li>
        </td>
        <td>
            <li>Publisher:
[Green-e](https://www.green-e.org/news)  </li>
            <li>represents US residual mix factors </li>
            <li>Envizi has managed this factor set since 2015 </li>
            <li>Can only be used in the  Envizi’s Market-based Emissions power report.</li>
        </td>
    </tr>
    <tr>
        <td>
[Residual Mix Emission Factors, AIB](https://knowledgebase.envizi.com/home/managed-emission-factors-aib-residual-mix-eu)
        </td>
        <td>
            <li> Australia           
           </li>
            <li>Market-based
            </li>
        </td>
        <td>
            <li>Scope 2 Market-based electricity</li>
        </td>
        <td>
            <li>Publisher: [Association of Issuing Bodies (AIB)](https://www.aib-net.org/facts/european-residual-mix)</li>
            <li>represents most EU countries' residual mix factors </li>
            <li>Envizi has managed this factor set since 2015 </li>
            <li>Can only be used in the  Envizi’s Market-based Emissions power report</li>
        </td>
    </tr>  
    <tr>
        <td>

[NGERS & National Greenhouse Accounts](https://knowledgebase.envizi.com/home/managed-emission-factors-aib-residual-mix-eu)
        </td>
        <td>
            <li> Applies at the country level for participating EU countries</li>
            <li>Market-based</li>
        </td>
        <td>
            <li>Scope 1: fossil fuels, biofuels, refrigerants</li>
            <li>Scope 2: Australian electricity</li>
            <li>Scope 3: upstream and downstream emissions resulting from Scope 1 and 2 emission sources, waste (very broad categories,  well-to-tank (upstream and downstream) emissions from Scope 3 activities </li>                        
        </td>
        <td>
            <li>Publisher: Australian Government. 2 factor sets </li>
            <li> 1) Scope 1, 2 Factors for [National Greenhouse and Energy Reporting (NGER) Act](https://www.legislation.gov.au/Series/F2008L02309) </li>
            <li> 2) Scope 3 indirect emission factors for [National Greenhouse Accounts (NGA)](https://www.industry.gov.au/data-and-publications/national-greenhouse-accounts-factors) </li>
            <li>Envizi has managed this factor set since 2009</li>
            <li>Envizi managed factor set is a combination of the direct factors from NGER and the indirect factors from the NGA workbooks</li>
            <li>NGER factors have specific reporting labels which assist in aligning Envizi’s NGER report outputs to match the input requirements for NGER reporters</li>
        </td>
    </tr>                    
    <tr>
        <td>
[New Zealand - Ministry for the Env.](https://knowledgebase.envizi.com/home/managed-emission-factors-new-zealand-ministry-for-)
        </td>
        <td>
            <li> New Zealand only
           </li>
            <li>Market-based
            </li>
        </td>
        <td>
            <li>Scope 1: fossil fuels, biofuels, refrigerants, passenger and delivery vehicles (distance based)</li>
            <li>Scope 2: NZ electricity : The yearly average figures provided are used in Envizi</li>
            <li>Scope 3: upstream and downstream emissions resulting from Scope 1 and 2 emission sources, working from home measured in employee/day, travel by vehicle size and distance, freight in tonne.km, water supply and waste water, waste, materials, agriculture and forestry </li>                        
        </td>
        <td>
            <li>Publisher: [New Zealand Ministry for the Environment](https://environment.govt.nz/publications/measuring-emissions-a-guide-for-organisations-2023-emission-factors-summary/) </li>
            <li> Envizi has managed this factor set since 2009 </li>

</li>
        </td>
    </tr>
    <tr>
        <td>

[USEEIO Emission Factors](https://knowledgebase.envizi.com/home/managed-emission-factors-supply-chain-greenhouse-g)
        </td>
        <td>
            <li>USA only
           </li>
        </td>
        <td>
            <li>Scope 3: Spend-based emission factors covering 394 commodities and 66 summary data types</li>
        </td>
        <td>
            <li>Publisher: [US EPA Supply chain GHG Emission factors for US Industries and Commodities](https://cfpub.epa.gov/si/si_public_record_Report.cfm?dirEntryId=349324&Lab=CESER) </li>
            <li>Envizi has managed this factor set since 2021</li>
            <li>factor set is managed using both raw figures with 2018 USD, and an inflation adjusted version</li>
</li>
        </td>
    </tr>     
    <tr>
        <td>US Climate Leaders
        </td>
        <td>
            <li>Applies to North America
           </li>
        </td>
        <td>
        </td>
        <td>
</li>
        </td>
    </tr>   
    <tr>
        <td>

Canada - National Inventory Factors
        </td>
        <td>
            <li>Canada
           </li>
        </td>
        <td>           
        </td>
        <td>
</li>
        </td>
    </tr>                    
</table>




## 5. How Emissions Factors are applied in Envizi ?

As we learnt in the beginning of the article, emissions are calculated for a given activity data  by applying the corresponding emission factor.  

### 5.1. Typical Emissions Factor selection process 

Let’s say, an organization in United States  purchases electricity from a electricity grid for their day to day operations. So here, `activity data = the electricity consumed` 

Now, how do we find which emission factor to apply on  this activity data(consumed electricity) to calculate the emissions?

Typically below steps are followed :

1. Check if Emission factors are provided by Supplier / Provider
2. If not,  look for available emission factors published for the regions, country, continent and global in sequence. 
    <img src="images/EM_Highlevel.png">    

Apart from what we see in the above diagram,  the organization may have other criteria to consider like choosing custom factors or standard factors, factor publishing date or effective date, etc. 
When the organization has operations spread across multiple regions / continents, it will be quite tedious and error prone process to find the applicable emission factor with so many criteria  to align with. That's when Envizi brings the value by automating the process to find the appropriate factor based by applying the Factor Selection Algorithm (FSA).  

### 5.1.2 How does the Factor selection works in Envizi? 

Assuming the data is loaded into Accounts / meters and normalized as Monthly data, Envizi apply the factor selection algorithm (FSA), which basically filters through the all available factors based on the following  five criteria: 
    
- **Data type** : The type of activity data such as Electricity, Natural Gas, etc.
- **Sub type** : Sub categorization similar to data type to link factors to accounts
- **Factor Set** : Collection of emission factors 
- **Region** : The region where the emission factor is applicable. 4 levels are considered (city, state, country, global)
- **Effective and Published Dates**: Organizations can apply factors by effective or published dates, depending on preference

Here is the pictorial representation of the same process.

<img src="images/Envizi_FSA.png">   

### 5.1.3 Factor Selection Algorithm with Example

Now, Lets look at how Emission factors are applied by Envizi. We have 3 examples below using the same `Account` and `Data type` but different `Location` and `Date`.
- Account - ELEC_VEEE1697
- Data type - Electricity

#### Example 1
- Location -  `New York, US`
- Date of Activity - Oct,2023
- Applied Factor - eGrid-2023
- Effective from - Jan 2021

<img src="images/Envizi-Electricity-NY_EMF-Details.png">    

#### Example 2
- Location -  `London Centre, UK`
- Date of Activity - `Dec, 2022 `
- Applied Factor - Managed DEFRA
- Effective from - Jan 2022

<img src="images/Envizi-Electricity-UK-Defra-2022.png">    

Between example 1 and 2 the locations are different so the emission factor applied is based on the Location.

#### Example 3

- Location -  London Centre, UK
- Date of Activity - `July, 2023`
- Applied Factor - Managed DEFRA
- Effective from - Jan 2023

<img src="images/Envizi-Electricity-UK-Defra-2023.png">    

- Between example 2 and 3 the `Locations` are same but `Date of Activity` is different. 
- Being the locations are same `DEFRA` Emission factor is applied for both.
- But versions of the `DEFRA` Emission factor is different because the `Date of Activity` is different.
- For example 2, `DEFRA-2022` factor set is applied because it is effective from `Jan 2022 - Dec 2022`.
- For example 3, `DEFRA-2023` factor set is applied which is effective from `Jan 2023`.
- You can also look at Total CO2e and Factor source values from the screenshot. 


### 5.1.4 Factors publishing dates

For keeping things easier and simpler, so far we only talk about Factor Effective dates, not publishing dates. To learn more on effective and published date logic works together in Envizi, please refer https://knowledgebase.envizi.com/home/factor-published-date-logic


## 6. How does these Emission Factor Sets are maintained in Envizi ?

Envizi product team follow the below steps to ensure factor appropriateness and correctness.

- Most current and up-to-date factors are available in the system 
- Ensure the data integrity by conducting  regular audits and reviews. 
- Set review dates for all factors which will be updating frequently
- Make sure no factor conflicts arises as the factor sets are being updated
- Create special list of factors based on the organization request
- Conducts variance analysis on factors which helps to find the factors exists outside the thresholds of datatypes. 


## 7. Custom Emission Factors

Envizi provides the standard set of emission factors with the platform. However, if your organization have defined custom emission factors, Envizi allows you to create the same in the platform. Once created, these custom factors are selected in preference to Envizi's default set of managed factors.

### 7.1. Create new Custom Factor 

To create new Custom Factor in Envizi, navigate to  `Admin -> Configuration -> Custom Factors` . 

Provide the inputs for the below parameters.
- **Region** : Provide the City / state / region for which the Custom factor should be applied
- **Data Type** : Choose the data type from the list
- **Factor Set** : Go with default. Nothing to update
- **Name** : Provide a unique name to represent the custom factor
- **Total CO2e** : Provide the emissions in CO2e 
- **Effective from** : Date from when this custom factor is applied
- **Effective to** : End date for the custom factor to be applied

<img src="images/Envizi-CF-Create-new.png">    

### 7.2. View the new Custom Factor 

Once created, you can view the Custom Emission Factors from the same page as `Admin -> Configuration -> Custom Factors`. 
    
Here is example of custom factors created in the system. In the below screenshot, you can see custom factors created for each `month` for the same `region` and `data type`.

<img src="images/Envizi-CF-list.png">    

Now, lets have a look at how these factors applied in Envizi. The custom factor would be applied to an account with the following.
- Data type : Natural Gas 
- Location : New South Wales, Australia.   

### 7.3. Custom Factor Examples

Below is the screenshot of the account's monthly data summary. For the Month of `March22`, the custom factor set `NSW_NG_Custom Factor-March22` is applied. You can also note the effective dates.

<img src="images/Envizi-CF-NSW-March22.png">  

Next, look at another monthly data record, where you can see a different custom factor is applied
`Envizi-CF-NSW-April22`

<img src="images/Envizi-CF-NSW-April22.png">  


## 8. Summary
    
In this article, we have discussed about the emission factors, what are the well-known emission factor sets available in public. We have also learnt how IBM Envizi uses Factor selection algorithm (FSA) to find the appropriate emission factor, how those factors are managed and maintained in Envizi. Lastly, we have learnt how Envizi supports organizations to create their own custom emission factors and apply the same for their activity data.
