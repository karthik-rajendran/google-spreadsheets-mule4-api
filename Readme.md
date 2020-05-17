
# google-sheets-api-connectivity-through-mule-api
This api has three operations such as read values from spreadsheets, append values in the spreadsheets and add a new sheet.
The spreadhseet id is configured in the application.properties

Operation 1:
# GET values/{range}
It will retrieve the values for a provided range in the uri param (like A1:C1) from the spreadsheet

Operation 2:
# POST values/{range}
It will append the values after the last non-empty rows
Sample request body
{
  "values": [
    [
      "05/10/2020",
      "Groceries",
      "1222"
    ]
  ]
}

Operation 3:
# POST sheets/
It will add a new sheet in the spreadsheet
