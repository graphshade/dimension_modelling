# Dimension Modelling for Data Warehouse


<h2>Project Description</h2>

CompanyX wants to create a structured data warehouse type solution, built on relational database technology, to support their operations department's analytical needs. 

CompanyX has a mature and well established transactional database that will be used to populate the data warehouse solution. The ERD of the transactional database is shown below.

<img src="https://i.imgur.com/Qj7aJIh.jpg" />



Notes about the analytical reporting needs of the group:

- Only data from completed orders will be moved to this data warehouse solution, so shipment information is complete. We do not need access to any of the shipment details except for two
calculations which we run all the time:  (a) how many boxes did it take to complete a specific order and (b) how many days went by between when the customer placed the order and when the final box was delivered (i.e., completion time).

- Order line item is an important set of data to us, as we need the ability to run reports about how much each item was sold as compared to the MSRP within the product table.

- We are really scrutinizing our vendors, so we find ourselves joining the vendor and product tables all the time. We only need the vendor name in these reports, so there might be a more efficient way to store the data.

<br/>
The task is to design a database solution that supports the specified OLAP uses, as opposed to a normalized solution that would be prudent for OLTP uses.


<h2>Proposed Solution</h2>

<img src="https://i.imgur.com/yYvycD9.jpg" />
