# Action Queue
Templates for an Action log implementation in GO

Options to implement an Action Log using GO

# What is it all about?

Often in a distributed environment you are in the situation that you want to manage asyncronous "actions" as requests to be send to distributed locations in an asynchrous manner, but you also want to manage the results of the actions in a reliable manner. You want t make sure, that actions are executed only once, but also you want to be able to track if an action was executed at all or with errors.

# Some Basic Assumptions
An "Action" is an indication of a function to be called in an asynchronous manner together with its parameters. 

It should be assumed that an "action" can be made to be idempotent, meaning executing an action twice should produce the same result - either by the function to be called is idempotent by itself or by just remembering the sucesful execution of the action at some leiable place

# Basics

# A Action Is Happening In Space and Time

To describe an action we at first want to give its instance a primary key. the primary key of an action should best be a "Transaction Sequence Number". 

# TSN

A TSN ("transaction sequence number") should uniquely define the starting point of ab "action". A "TSN"is the outcome of a kind of a wall clock. There can be many clocks, but a single clock is to be used to describe a sequence of related operations. 



