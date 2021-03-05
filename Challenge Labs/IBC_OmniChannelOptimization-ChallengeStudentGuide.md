<!--!
[](--logo link-- 'Microsoft Industry-Based Challenges')
-->
# Industry-Based Challenges: Omni-Channel Optimization  

## Challenge lab student guide  

### March 2021  

Information in this document, including URL and other Internet Web site references, is subject to change without notice. Unless otherwise noted, the example companies, organizations, products, domain names, e-mail addresses, logos, people, places, and events depicted herein are fictitious, and no association with any real company, organization, product, domain name, e-mail address, logo, person, place or event is intended or should be inferred. Complying with all applicable copyright laws is the responsibility of the user. Without limiting the rights under copyright, no part of this document may be reproduced, stored in or introduced into a retrieval system, or transmitted in any form or by any means (electronic, mechanical, photocopying, recording, or otherwise), or for any purpose, without the express written permission of Microsoft Corporation.

Microsoft may have patents, patent applications, trademarks, copyrights, or other intellectual property rights covering subject matter in this document. Except as expressly provided in any written license agreement from Microsoft, the furnishing of this document does not give you any license to these patents, trademarks, copyrights, or other intellectual property.

The names of manufacturers, products, or URLs are provided for informational purposes only and Microsoft makes no representations and warranties, either expressed, implied, or statutory, regarding these manufacturers or the use of the products with any Microsoft technologies. The inclusion of a manufacturer or product does not imply endorsement of Microsoft of the manufacturer or product. Links may be provided to third party sites. Such sites are not under the control of Microsoft and Microsoft is not responsible for the contents of any linked site or any link contained in a linked site, or any changes or updates to such sites. Microsoft is not responsible for webcasting or any other form of transmission received from any linked site. Microsoft is providing these links to you only as a convenience, and the inclusion of any link does not imply endorsement of Microsoft of the site or the products contained therein.

© 2020 Microsoft Corporation. All rights reserved.

Microsoft and the trademarks listed at <https://www.microsoft.com/legal/intellectualproperty/Trademarks/Usage/General.aspx> are trademarks of the Microsoft group of companies. All other trademarks are property of their respective owners.

# Omni-Channel Optimization challenge lab student guide

## Abstract and learning objectives

Parts Unlimited, a subsidiary of Fabrikam Retail INC., has been feeling some pain and would like your help to redesign and implement some new solutions to be able to better compete in the current marketplace.  Among the main problems that Parts Unlimited is facing are 

*   Lack of connection between online and in-store data leading to an inability to provide a selection optimization that is tailored to a specific customer
*   Inconsistent pricing, promotion, product availability, and fulfillment strategies exist across their various channels
*   Customers are not completing orders due to redundant steps in the shopping journey, and encountering irrelevant interactions with the system
*   Currently, Parts Unlimited is unable to address latent customer needs
*   Parts Unlimited is unable to deliver an engaging and compelling experience to their customers regardless of platform or location.
*   Customer experiences vary when shopping across channels, including having fragmented and inconsistent experiences. 
*   Parts Unlimited currently is unable to maximize the effectiveness of their workforce.

To remedy this solution, Parts Unlimited is asking you to deliver a solution that will allow their customers to experience a smooth and relevant experience, regardless of the platform, device, and/or channel from which they are shopping. Of great importance is the ability to deliver dynamic and rich content that includes augmented and mixed-reality experiences.  Furthermore, customer data should be used to present relevant shopping experiences and product consistency to delight their customers. 

Parts Unlimited wants to ensure that they have maximized their ad spend for increased ROI and increased revenue.  Additionally, Parts Unlimited wants their customers to have an engaging experience that is similar on all digital channels and in their brick-and-mortar stores. 

An additional piece of information Parts Unlimited would like is the ability to be able to optimize the utilization and effectiveness of their workforce.  

In the end, your solution should provide a vision that allows the audience (the Chief Marketing Officer, Chief Digital Officer, the Chief Data Officer, and the Customer Experience Manager) to understand how using this solution will give the information that is needed to deliver the Omni-Channel optimized solution. 

## Customer case study

### Customer situation

Parts Unlimited Retail, Inc has been selling goods through various retail channels for the past 15 years.  As various platforms and technologies have evolved, Parts Unlimited has struggled to keep up, but has done the best they could to continue to provide solutions for their customers.  

Currently, they have just over 200 brick-and-mortar stores but are planning to close 50+ of these stores next year, taking the number of physical locations down to 150 stores due to declining revenue and various other factors.  Of the remaining 150 stores, 35 of them are currently streamlined for an attempted re-branding that happened a few years ago.  The re-branded stores were chosen based on population bases of less than 50,000 in an 200 square mile radius or within 50 miles of a major metropolitan area. These rebranded "Parts Unlimited Hometown" stores eliminated most of the non-essential retail, such as sporting and workout equipment, and focused in on essentials like appliances, automotive, and kept a limited selection of electronics, only offering about 15% of the options for items like UHD televisions, antennas, and blu-ray players.  Customers have expressed frustrations when an advertisement in the local newspaper for Parts Unlimited included a great deal on a large-screen television only to find they have to order online or drive to the larger store in a city that is sometimes located over 50 miles away.  While it is clear that customers are not pleased with this solution, it is not clear if this is an effective strategy to save the company when it comes to providing a simplified retail option. 

In addition to re-branding efforts, in the past few years attempts have been made to enhance the web app for responsive delivery and a couple of apps were also built to specifically target IOS and Android devices. Unfortunately, the data from these applications and the web solution is not connected, and when a user switches devices or goes from a device to the web, the experience is not uniform, leading to confusion and frustration.  Questions such as "why isn't the item I selected on my phone in my cart when I go to the website?" are far too common.    

Parts Unlimited needs an ability to collect and analyze all of this data in order to make the best uniform solution possible.   The solution needs to allow for a user to be able to walk into a brick-and-mortar store and get the items they are looking for, or to be able to switch from any device to the web or from the web to a device and get a streamlined experience.  Finally, the customer needs to leave the shopping experience as an advocate for the company, having been delivered an experience that they would recommend to others.   

#### Customer's current process

Parts Unlimited currently has over 200 brick-and-mortar stores, with 50+ stores closing and 35 stores running the re-branded profile.  Some stores have a pre-determined, limited selection and a limited inventory of the products they do offer. 

Parts Unlimited has an MVC website written in the .Net Framework and has been previously upgraded to version 4.7.2. The website is supposed to be responsive, as it utilized Bootstrap for responsive layout, but the site is currently not able to work on a few devices due to some styling problems.  

In addition to the website, Parts Unlimited has an Android application written in native Java that is three versions behind the current version of Android, but has been upgraded enough to continue to work on newer devices, even though it does not necessarily leverage all of the features of newer devices.  

Along with the website and android app, a third app written in Swift is available for use on the Apple IOS devices.  

All applications and sites do work, but the user experience, including sign-on, shopping cart, and other factors is unique to each platform.  For example, a user must sign in on the website and then sign in again on the device, and the shopping cart is not shared across devices, so items added to the cart on the web do not show up on the phone, or vice-versa.

As a struggling retailer, Parts Unlimited has a limited amount of resources to apply to getting the entire experience upgraded, so they need you to come up with the best, cost-effective solution.   

### Current Process
![High level view of the current process](media/omnichannel/CurrentProcess.png 'Current process diagram') 
 

### Customer needs

1. Deliver a seamless experience to the user, regardless of platform, device, or location (online or at brick-and-mortar traditional stores)

2. Use customer data to deliver a relevant shopping experience.

3. Provide a customer experience on any delivery that provides dynamic and rich content. 

4. Present relevant and consistent product information to the customers, including using customer data to choose relevant products, remove any redundant or unnecessary interactions.  Make the customer feel unique and valued through the experience.

5. Ensure that pricing, promotions, product availability are all consistent and easy to manage so that the experience is the same on all channels. 

6. Respond to customer needs, including the ability to fulfill latent customer needs. 

### Infographic for common scenarios
 
![Infographic for common scenarios](media/omnichannel/common-scenarios-iot.png 'Common scenarios diagram') 

_High-level architecture_

1. Challenges will require you to build the environment to meet the customer requirements outlined above.  It should include: 

*   Ingestion of data
*   What solutions for ETL or ELT
*   Organization and/or filtering of data
*   Presentation of data


## Challenge 1: Build the architecture for collecting and ingesting (extract) data

   >**Note**: Complete the Before HOL setup prior to proceeding to the challenge tasks below. Provide this link to participants to access the setup instructions.
<https://github.com/msusdev/Industry-Omni-Channel/blob/main/Challenge%20Labs/BeforeTheChallenge/BeforeTheChallenge.md>

_Data ingest_

1. What are your recommended options for ingesting payment transaction events and customer shopping data as they occur in a scalable way that can be easily processed while maintaining event order with no data loss?

2. Of the ingest options you identified previously, which would you recommend for Parts Unlimited's scenario?

### Success criteria

-	Determine and build the architecture for collecting data into Azure:

    o	On-premises data: customer information, inventory, sales/POS

    o	Online data: customer information, inventory, sales/POS

    o	Workforce optimization data: number of staff each shift, customers per hour

    o	Cost efficiency data: what products are being viewed and purchased most, and by what demographic (location, visitor persona, etc.)

    o	Online traffic and sources to the website (social media, search engines, direct email marketing, mobile app, etc.)

-	Determine and build the architecture for where to ingest data into Azure


## Challenge 2: Build the architecture for loading and transforming data

_Data transformation_

1. What solutions offer options for ETL and/or ELT?  

2. Which option would you recommend and why?

_Data processing_

1. How will you filter the data to get relevant information?

2. How will you ensure that data processes are repeatable?

### Success criteria

-	Determine and build the architecture for loading the data

    o	Understand what data is being collected and what form

    o	Is the data collected in a hot or cold path, and how would each be loaded into Azure
    - Does any of this data need to be accessible in near real-time?

    o	Design the architecture for real-time and monthly data use from the website
    


## Challenge 3: Build the architecture for presenting the data

_Dashboards and reporting_

1. Parts Unlimited's business analysts would like to have a set of dashboards they can monitor that provide real-time views of customer data. What do you propose using to meet this requirement? Be specific about how this solution will be put in place and which features it supports, and why it will be useful to the business analysts.

2. Parts Unlimited's data analysts, who build and maintain reports, are comfortable working with T-SQL. How can they efficiently access the data for analytical queries, ensuring they have access to the most up-to-date data, without impacting the transactional data store?

### Success criteria

-	Determine and build the architecture for presenting the data

    o	Provide a dashboard for business users to be able to review data and make informed decisions

    o	Dashboard should include:
    
    - Sales data for stores and online with a comparison
    - Navigation habits for online customers
    - Purchase and view habits of in person customers
    - Digital marketing and social media effectiveness based on campaigns, traffic to the website, and online sales.
    - Recommendations on products that gain the most traffic by location and demographic

    o	Data should be updated within the dashboard in near real-time based on the frequency of data that is collected.


## Additional references

| **Description**                                        | **Links**                                                                                                                         |
| ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------- |
| Create a data factory                              | <https://docs.microsoft.com/en-us/azure/data-factory/quickstart-create-data-factory-portal>                                                                         |
| Load data into Azure Data Lake Storage from Azure Data Factory               | <https://docs.microsoft.com/en-us/azure/data-factory/load-azure-data-lake-storage-gen2>                                                                         |
| Azure Data Explorer data ingestion overview        | <https://docs.microsoft.com/en-us/azure/data-explorer/ingest-data-overview>                                                                         |
| What is Azure Databricks        | <https://docs.microsoft.com/en-us/azure/databricks/scenarios/what-is-azure-databricks>                                                                         |
| Azure Synapse Analytics        | <https://azure.microsoft.com/en-us/services/synapse-analytics/>                                                                         |
| Using Synapse analytics from Databricks        | <https://docs.microsoft.com/en-us/azure/databricks/data/data-sources/azure/synapse-analytics>                                                                         |
| Using SQL file metadata in synapse analytics        | <https://docs.microsoft.com/en-us/azure/synapse-analytics/sql/query-specific-files>                                                                         |

