API Collections
###############

Account Receivable 
******************

Summary
=======

==============================  ==========================
Operations                      Description
==============================  ==========================
GET/getTotalNumberOfInvoices    Get Total number of invoices.
GET/getTopARCustomers           Get Top Account Receivable Customers.
GET/getInvoiceOutstandingDue    Get Total Invoice Outstanding Due Amount.
GET/getDSO                      Get DSO details.
GET/getMapInvoiceStatus         Get Map Invoice Status details.
GET/getOpenInvoiceDetails       Get Open Invoice Details.
==============================  ==========================


End Points
==========
**Total Invoices By Month**: 

``GET /getTotalNumberOfInvoices``
    
    Retrive Total number of invoices.
    
**Parameters :**

    **Year(Optional)** : Year parameter as 2015,2016,2017.  
    
    **Entity(Optional)** : Entity Name parameter such as Infometry.
    
    **Customer Name(Optional)** : Customer Name parameter such as Better Buy,DelRey Distributors.
        
 
**Example Response**:

    .. sourcecode:: json

        {
            "2015": null,
            "2016": null,
            "2017": 107,
            "Month_of_Date_Created":Jan
        },
        {
            "2015": null,
            "2016": null,
            "2017": 107,
            "Month_of_Date_Created":Jan
        }
        
        
        
**Top AR by Customers**:        
    
``GET /getTopARCustomers``

    Retrive all Top Account Receivable Customers.
    
**Parameters :**

    **Year(Optional)** : Year parameter as 2015,2016,2017.  
    
    **Entity(Optional)** : Entity Name parameter such as Infometry.
    
    **Customer Name(Optional)** : Customer Name parameter such as Better Buy,DelRey Distributors.
        
**Example Response**:

    .. sourcecode:: json

        {
            "CUSTOMER_NAME": "DelRey Distributors",
            "AMOUNT": "$1,955K"
        },
        {
            "CUSTOMER_NAME": "Everett Fine Wines",
            "AMOUNT": "$1,728K"
        }
        
        
        
**Invoices Outstanding Due**:        
    
``GET /getInvoiceOutstandingDue``
   
    Get Total Invoice Outstanding Due Amount.
    
**Parameters :**

    **Year(Optional)** : Year parameter as 2015,2016,2017.  
    
    **Entity(Optional)** : Entity Name parameter such as Infometry.
    
    **Customer Name(Optional)** : Customer Name parameter such as Better Buy,DelRey Distributors.
    
        
**Example Response**:

    .. sourcecode:: json

        {
            "CUSTOMER_NAME": "DelRey Distributors",
            "INVOICES_CLEARED": "450.0",
            "TOTAL_OUTSTANDING_INVOICES": "171.0"
        },
        {
            "CUSTOMER_NAME": "Better Buy",
            "INVOICES_CLEARED": "61.0",
            "TOTAL_OUTSTANDING_INVOICES": "4.0"
        }


**DSO yearwise**:
    
``GET /getDSO``

    Retrive Total DSO details yearwise.
    
**Parameters :**

    **Year(Optional)** : Year parameter as 2015,2016,2017.  
    
    **Entity(Optional)** : Entity Name parameter such as Infometry.
    
    **Customer Name(Optional)** : Customer Name parameter such as Better Buy,DelRey Distributors.
    
        
**Example Response**:

    .. sourcecode:: json

        {
            "YEAR_OF_INVOICE_DATE": 2015,
            "DSO": "181"
        },
        {
           "YEAR_OF_INVOICE_DATE": 2016,
            "DSO": "182"
        }
        
**Month Invoices Satus**:
    
``GET /getMonthInvoiceStatus``
    
    Get all Map Invoice Status details.
    
**Parameters :**

    **Year(Optional)** : Year parameter as 2015,2016,2017.  
    
    **Entity(Optional)** : Entity Name parameter such as Infometry.
    
    **Customer Name(Optional)** : Customer Name parameter such as Better Buy,DelRey Distributors.
    
        
**Example Response**:

    .. sourcecode:: json

        {
            "YEAR_OF_INVOICE_DATE": 2015,
            "DSO": "181"
        },
        {
           "YEAR_OF_INVOICE_DATE": 2016,
            "DSO": "182"
        }
        

**Open Invoices Details**:
    
``GET /getOpenInvoiceDetails`` 
    
    Get Open Invoice Details.
 
 **Parameters :**

    **Year(Optional)** : Year parameter as 2015,2016,2017.  
    
    **Entity(Optional)** : Entity Name parameter such as Infometry.
    
    **Customer Name(Optional)** : Customer Name parameter such as Better Buy,DelRey Distributors.
        
        
**Example Response**:

    .. sourcecode:: json

        {
            "YEAR_OF_INVOICE_DATE": 2015,
            "DSO": "181"
        },
        {
           "YEAR_OF_INVOICE_DATE": 2016,
            "DSO": "182"
        }
 
 

Income and Expense Analysis 
***************************

Summary
=======

==============================  ==========================
Operations                      Description
==============================  ==========================
GET/getExpensesByMonth          Get Expenses By Month.
GET/getOpExRevenueRatio         Get OpEx to Revenue Ratio.
GET/getIncomeExpenses           Get Income and Expenses.
==============================  ==========================


End Points
==========

``GET/getExpensesByMonth``

    Get Total Expenses By Month details.
    
``GET/getOpExRevenueRatio``

    Get OpEx to Revenue Ratio details.

``GET/getIncomeExpenses``

    Get Total Income and Expenses details.
    

Liquidity Analysis 
******************

Summary
=======

==============================  ==========================
Operations                      Description
==============================  ==========================
GET/getCashAndAR                Get Cash And AR.
GET/getTopARCustomers           Get Top Account Receivable By Customers.
GET/getARbyCompany              Get Account Receivable By Company.
GET/getAPbyCompany              Get AP By Company details.
==============================  ==========================


End Points
==========

``GET/getCashAndAR``

    Get Total number of Cash And AR details.

``GET/getTopARCustomers``

    Get all Top Account Receivable By Customers.
 
``GET/getARbyCompany``

    Get Account Receivable By Companydetails.

``GET/getAPbyCompany``

    Get AP By Company details..


AccountReceivable Analysis
**************************

Summary
=======

==============================  ==========================
Operations                      Description
==============================  ==========================
GET/getARbyCity                 Get Account Receivable by City.
GET/getOutstandingbyCompany     Get Outstanding By Company.
GET/getARbyInvoiceNumber        Get AR By Invoice Number.
GET/getOpenInvoices             Get Open Invoices.
==============================  ==========================


End Points
==========

``GET/getARbyCity``

    Get Total Account Receivable by City details.
    
``GET/getOutstandingbyCompany``

    Get Total Outstanding By Company details.

``GET/getARbyInvoiceNumber``

    Get Total AR By Invoice Number details.
    
``GET/getOpenInvoices``

    Get Total Open Invoices details.    
    
    
Profitability Analysis
**********************

Summary
=======

================================  ============================
Operations                        Description
================================  ============================
GET/getGrossProfitByItems         Get Gross Profit By Items.
GET/getTop20ItemsByRevenue        Get Top 20 items By Revenue.
GET/getNetProfitTrend             Get Net Profit Trend.
GET/getProfitabilityDescription   Get Profitability Description.
GET/getGrossProfitByProductLine   Get Gross Profit by ProductLine.
GET/getCOGSByProductLine          Get COGS by ProductLine.
GET/getRevenueByProductLine       Get Revenue by ProductLine.
GET/getOperationalExpences        Get Operational Expences by items.
================================  ============================


End Points
==========

``GET/getGrossProfitByItems``

    Get Gross Profit By Items details.

``GET/getTop20ItemsByRevenue``

    Get Top 20 items By Revenue details.
    
``GET/getNetProfitTrend``

    Get Net Profit Trend details.    
    
``GET/getProfitabilityDescription``

    Get Profitability Description details.   
    
``GET/getGrossProfitByProductLine``

    Get Gross Profit by ProductLine details.   
    
``GET/getCOGSByProductLine``

    Get COGS by ProductLine details.  
    
``GET/getRevenueByProductLine``

    Get Revenue by ProductLine details.
    
``GET/getOperationalExpences``

    Get Operational Expences by items details.    
    
    
Budget Detail
*************

Summary
=======

==============================  ==========================
Operations                      Description
==============================  ==========================
GET/getExpenses                 Get Expenses.
GET/getRevenue                  Get Revenue.
GET/getDepartmentalExpenses     Get Departmental Expenses.
GET/getExpensesVariance         Get Expenses Variance.
GET/getRevenueVariance          Get Revenue Variance.
==============================  ==========================


End Points
==========

``GET/getExpenses``

    Get Expenses details.

``GETgetRevenue``

    Get Revenue details.
    
``GET/getDepartmentalExpenses``

    Get Departmental Expenses details.
    
``GET/getExpensesVariance``

    Get Expenses Variance details.    
    
``GET/getRevenueVariance``

    Get Revenue Variance details.    
    
    

Account Payable Analysis
************************

Summary
=======

==============================  ==========================
Operations                      Description
==============================  ==========================
GET/getTopCreditors             Get Top Creditors.
GET/getPaymentProcessEvolved    Get Payment Process Evolved.
==============================  ==========================


End Points
==========

``GET/getTopCreditors``

    Get Top Creditors details.
    
``GET/getPaymentProcessEvolved``

    Get Payment Process Evolved details.



