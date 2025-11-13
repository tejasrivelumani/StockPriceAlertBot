Stock Price Alert Bot (UiPath Project)



1.Overview

The Stock Price Alert Bot is an automation solution developed in UiPath Studio that monitors live stock prices from Yahoo Finance.
When the stock price falls below a user-defined threshold, it automatically triggers a notification alert, removing the need for manual monitoring.



2.Key Features

Automates live stock data extraction from Yahoo Finance

Compares current price with a user-set threshold

Displays instant alerts when conditions are met

Uses a modular and reusable UiPath workflow design



3.Technologies Used

UiPath Studio (Community Edition)

RPA Concepts – Variables, Selectors, Assign, Message Box

Regex – String-to-numeric conversion

Yahoo Finance – Data source



4.How It Works

Opens Yahoo Finance for the selected stock.

Extracts and converts the stock price into a numeric format.

Compares it against the user-defined threshold.

Displays an alert message if the price is below the limit.



5.Example Code Snippet

Here’s a simplified version of the bot’s core logic in VB (used in UiPath Assign and If activities):

' Extract and clean the price text
currentPrice = CStr(System.Text.RegularExpressions.Regex.Replace(yourValue, "[^\d.]", ""))

' Convert to numeric
currentPriceNum = CDbl(currentPrice)

' Compare and alert
If currentPriceNum < threshold Then
    MessageBox.Show("Stock price is below threshold!")
End If

  

6.Learning Highlights

Real-world application of RPA in finance

Hands-on experience with selectors and data handling

Workflow design for efficiency and reliability



7.Future Enhancements

Email or SMS-based alerts

Multi-stock monitoring

Automated daily stock report generation




Author


Teja Sri V

AI & Data Science Enthusiast 
GitHub: https://github.com/tejasrivelumani

LinkedIn: https://www.linkedin.com/in/teja-sri-v-b996b8310
