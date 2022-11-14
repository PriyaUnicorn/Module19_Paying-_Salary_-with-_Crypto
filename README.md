# Module19_Paying-_Salary_-with-_Crypto


📌 Challenge 19

> "In this Challenge, I assumed the role of blockchain lead developer, working for a fintech startup. My goal is to integrate the Ethereum blockchain network into Fintech Finder application in order to enable customers to instantly pay the fintech professionals whom they hire with cryptocurrency. "


## Overview of the project 

In this Challenge, I was task to  complete the code that enables customers to send cryptocurrency payments to fintech professionals. To develop the code and test it out, we assume the perspective of a Fintech Finder customer who is using the application to find a fintech professional and pay them for their work.

To complete this Challenge, I am using two Python files:
1. [fintech_finder.py]()  contains the code associated with the web interface of the application. The code included in this file is compatible with the Streamlit library. 

2. [crypto_wallet.py]() contains the Ethereum transaction functions. By using import statements, I integrate the crypto_wallet.py Python script into the Fintech Finder interface program that is found in the fintech_finder.py file. 


Integrating these two files allow the user to automate the tasks associated with generating a digital wallet, accessing Ethereum account balances, and signing and sending transactions via Ganache Application.

## Project steps

The steps for this Challenge are divided into the following sections:

### Step 1: Import Ethereum Transaction Functions into the Fintech Finder Application

##### Import generate_account, get_balance, and send_transaction from the crypto_wallet.py file. 

<img width="677" alt="Screen Shot1" src="https://user-images.githubusercontent.com/108702820/201551801-873e1f4a-0244-456b-a99c-c73b84842ef1.png">

##### Call the generate_account function and store the account object. 

<img width="641" alt="Screen Shot 2021-08-04 at 4 03 48 PM" src="https://user-images.githubusercontent.com/80833988/128266414-580b51f1-edf8-4ad8-856e-900a1aae9731.png">

##### Call the get_balance function and pass it the Ethereum account.address. 

<img width="540" alt="Screen Shot 2021-08-04 at 4 05 12 PM" src="https://user-images.githubusercontent.com/80833988/128266512-98987639-4727-4d10-88c9-afbb3e35a7ba.png">


### Step 2: Sign and Execute a Payment Transaction

##### Calculate the transaction’s total wage. 

<img width="649" alt="Screen Shot 2021-08-04 at 4 08 53 PM" src="https://user-images.githubusercontent.com/80833988/128266856-bc69f876-0114-4fa6-8d83-2f259d90ea49.png">


##### Call the send_transaction function and pass it the account, candidate_address, and wage parameters. 
<img width="620" alt="Screen Shot 2021-08-04 at 4 07 07 PM" src="https://user-images.githubusercontent.com/80833988/128266681-032720a8-1dbe-41c8-a11b-fb3fc2a4a9ed.png">


##### Return the transaction hash from the send_transaction and display it on the application’s web interface. 

<img width="327" alt="Screen Shot 2021-08-04 at 4 23 43 PM" src="https://user-images.githubusercontent.com/80833988/128267978-dbeb83fb-1dcf-4a1b-9afa-95736b6b9d50.png">



### Step 3: Inspect the Transaction on Ganache Application.

##### Send a transaction using the Fintech Finder app


![Video Recording of Send Transaction]("https://myoctocat.com/assets/images/Screen Recording 2022-11-13 at 6.49.18 PM.mov")


##### Provide screenshots from Ganache that show the sender’s address balance and history, and the recipient's address balance and history.

<img width="1391" alt="Ganache" src="https://user-images.githubusercontent.com/108702820/201552022-e5d93186-4041-4578-9723-06169dfab905.png">


## Software version control


### Libraries 

##### Following libraries were imported

* crypto_wallet.py

[
<img width="658" alt="Screen Shot 2021-08-02 at 1 05 59 PM" src="https://user-images.githubusercontent.com/80833988/127917395-947eaeaf-7ade-471f-84ec-e96e3c8eafa4.png">
](url)

* fintech_finder.py

```
# Import the required libraries and dependencies


import streamlit as st
from dataclasses import dataclass
from typing import Any, List

```

* Streamlit- is an open-source app framework for Machine Learning and Data Science teams.
* Dataclasses-a utility tool to make structured classes specially for storing data. These classes hold certain properties and functions to deal specifically with the data and its representation.
* Typing-provides runtime support for type hints. The most fundamental support consists of the types Any, Union, Tuple, Callable, TypeVar, and Generic.



