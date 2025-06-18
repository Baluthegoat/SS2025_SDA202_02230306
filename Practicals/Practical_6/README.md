## Bounded Context

1. Account Management : handles different types of account.
2. Customer Management : manages customer information 
3. Branch Management : manages branch information

## Aggregates

1. Customer Aggregate.
    
    Entity : Customer, ATM card 
    
    Customer Attributes : ID, Name, Address, Employment details, Account number, ATM card ( optional ).
    
    ATM card Attributes : ID, Customer ID, Date of issue.
    
    Value Object : Employment details
    
    Employment details Attributes : Company name, Telephone number, Annual salary range, Occupation, Designation 
    
2. Account Aggregate.
    
    Root Entity : Account 
    Entity : Saving account, Current account.
    
    value object : account type
    
    Account Attributes : Account number, Account type, Holder ID, Joint holder ID, Branch name, Balance.
    
    Saving account attributes : Minimum balance.
    
    Current account attributes : Linked saving account number
    

1. Branch Aggregate.
    
    Entity : Branch
    
    Branch Attributes : Branch name, Address
    

**Domain objects : Customer, employment details, ATM card, Account, saving account, current account, Branch.**

## Relationships / association of relevant Domain objects

**Customer Aggregate :** 

1. Customer is the root entity with the attributes and value object ( employment details ).
2. Customer has one-to-many association with Account, where a customer can have unlimited number of account.
3. Customer has one-to-one association with ATM card but it is optional. Customer can remain active even after terminating the ATM card. 

**Account Aggregate :** 

1. Account is the root entity
2. Account has many-to-one association with customer, each account can have one or many holders
3. Account has many-to-one association with Branch

**Branch Aggregate :** 

1. Branch has one-to-many association with Account, where one branch can have many accounts