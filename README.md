# Performance Testing - 

## Project Description
This project is based on Performance Testing of the Dmoney API using Apache JMeter.
In this project:
- 5 agents performed deposit transactions for 10 customers
- 5 customers sent money to another 10 customers
- 5 customers made payments to 2 merchants
- Separate Thread Groups were created for:
  - Deposit
  - Send Money
  - Payment
- Dynamic transaction amounts were generated using Random Variable Controller
- CSV Data Set Config was used for handling multiple accounts
- Assertions were added to validate successful transactions
- HTML performance report was generated using JMeter

## Technology Used
- Apache JMeter
- CSV Data Set Config
- Random Variable Controller
- HTML Dashboard Report

## Test Scenario

### Deposit
5 Agents deposit money to 10 Customers

### Send Money
5 Customers send money to another 10 Customers

### Payment
5 Customers make payments to 2 Merchants
Ramp-up Time for each Thread Group: **120 seconds**

## Resources
- `testing.jmx`
- `deposit.csv`
- `sendMoney.csv`
- `payment.csv`

## How to Run
jmeter -n -t testing.jmx -l testing.jtl -e -o Reports

## Screenshot of Report
<img width="1897" height="910" alt="test1" src="https://github.com/user-attachments/assets/4f886286-04af-41f8-90a7-227ba4cc277d" />
<img width="1902" height="957" alt="test2" src="https://github.com/user-attachments/assets/54ca4a92-00ef-411d-b9b4-adf0ef06386b" />




