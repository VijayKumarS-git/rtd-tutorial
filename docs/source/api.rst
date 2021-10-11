Summary :-


Operation	Description
GET/getTotalNumberOfInvoices	Get Total number of invoices.
GET/getIncomeExpenseData	Get Total Income Expense Data
GET/getTopARCustomers	Get all Top Account Receivable Customers
GET/getInvoiceOutstandingDue	Get all Invoice Outstanding Due Amount
GET/getDSO	Get Total DSO


End Points:-

GET/getTotalNumberOfInvoices

Get Total number of invoices.

Example Request:-
http://localhost:3000/getTotalNumberOfInvoices

Example Response:- 

[
    {
        "2015": null,
        "2016": null,
        "2017": "107",
        "MONTH_OF_DATE_CREATED": "Jan"
    },
    {
        "2015": null,
        "2016": null,
        "2017": "35",
        "MONTH_OF_DATE_CREATED": "Mar"
    },
    {
        "2015": null,
        "2016": null,
        "2017": "30",
        "MONTH_OF_DATE_CREATED": "Apr"
    },
    {
        "2015": "28",
        "2016": null,
        "2017": null,
        "MONTH_OF_DATE_CREATED": "Jun"
    },
    {
        "2015": "24",
        "2016": null,
        "2017": null,
        "MONTH_OF_DATE_CREATED": "Jul"
    },
    {
        "2015": null,
        "2016": null,
        "2017": "8",
        "MONTH_OF_DATE_CREATED": "Aug"
    },
    {
        "2015": null,
        "2016": null,
        "2017": "3",
        "MONTH_OF_DATE_CREATED": "Oct"
    },
    {
        "2015": null,
        "2016": "974",
        "2017": null,
        "MONTH_OF_DATE_CREATED": "Nov"
    },
    {
        "2015": "13",
        "2016": "4594",
        "2017": null,
        "MONTH_OF_DATE_CREATED": "Dec"
    }
]



GET/getTopARCustomers

Get all Top Account Receivable Customers.

Example Request:-
http://localhost:3000/getTopARCustomers


Example Response:- 

[
    {
        "CUSTOMER_NAME": "DelRey Distributors",
        "AMOUNT": "$1,955K"
    },
    {
        "CUSTOMER_NAME": "Everett Fine Wines",
        "AMOUNT": "$1,728K"
    },
    {
        "CUSTOMER_NAME": "B-Sharp Music",
        "AMOUNT": "$800K"
    },
    {
        "CUSTOMER_NAME": "Anderson Boughton Inc.",
        "AMOUNT": "$751K"
    },
    {
        "CUSTOMER_NAME": "Academy Sports & Outdoors",
        "AMOUNT": "$705K"
    },
    {
        "CUSTOMER_NAME": "Better Buy",
        "AMOUNT": "$583K"
}
]


GET/getInvoiceOutstandingDue

Get all Invoice Outstanding Due Amount.

Example Request:-
http://localhost:3000/getInvoiceOutstandingDue


Example Response:- 

[
    {
        "CUSTOMER_NAME": "TAX",
        "INVOICES_CLEARED": "450.0",
        "TOTAL_OUTSTANDING_INVOICES": "171.0"
    },
    {
        "CUSTOMER_NAME": "DelRey Distributors",
        "INVOICES_CLEARED": "90.0",
        "TOTAL_OUTSTANDING_INVOICES": "6.0"
    },
    {
        "CUSTOMER_NAME": "Better Buy",
        "INVOICES_CLEARED": "61.0",
        "TOTAL_OUTSTANDING_INVOICES": "4.0"
    },
    {
        "CUSTOMER_NAME": "Jason Paul Distribution",
        "INVOICES_CLEARED": "51.0",
        "TOTAL_OUTSTANDING_INVOICES": "3.0"
    },
    {
        "CUSTOMER_NAME": "Smith Inc.",
        "INVOICES_CLEARED": "49.0",
        "TOTAL_OUTSTANDING_INVOICES": "19.0"
    },
    {
        "CUSTOMER_NAME": "Selders Distributors",
        "INVOICES_CLEARED": "48.0",
        "TOTAL_OUTSTANDING_INVOICES": "3.0"
    },
    {
        "CUSTOMER_NAME": "Academy Sports & Outdoors",
        "INVOICES_CLEARED": "31.0",
        "TOTAL_OUTSTANDING_INVOICES": "0.0"
    },
    {
        "CUSTOMER_NAME": "Smith Inc. : Smith East",
        "INVOICES_CLEARED": "25.0",
        "TOTAL_OUTSTANDING_INVOICES": "2.0"
    },
    {
        "CUSTOMER_NAME": "Smith Inc. : Smith West",
        "INVOICES_CLEARED": "19.0",
        "TOTAL_OUTSTANDING_INVOICES": "3.0"
    },
    {
        "CUSTOMER_NAME": "Sports Authority",
        "INVOICES_CLEARED": "12.0",
        "TOTAL_OUTSTANDING_INVOICES": "1.0"
    },
    {
        "CUSTOMER_NAME": "Harriage Plumbing Dynamics",
        "INVOICES_CLEARED": "9.0",
        "TOTAL_OUTSTANDING_INVOICES": "1.0"
}
]




GET/getDSO

Get Total DSO.

Example Request:-
http://localhost:3000/getDSO


Example Response:- 

[
    {
        "YEAR_OF_INVOICE_DATE": "2015",
        "DSO": "181"
    },
    {
        "YEAR_OF_INVOICE_DATE": "2016",
        "DSO": "182"
    },
    {
        "YEAR_OF_INVOICE_DATE": "2017",
        "DSO": "8,276"
    }
]


