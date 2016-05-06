# Action Queue
Templates for an Action log implementation in GO

Options to implement an Action Log using GO

# What is it all about?

Often in a distributed environment you are in the situation that you want to manage asyncronous "actions" as requests to be send to distributed locations in an asynchrous manner, but you also want to manage the results of the actions in a reliable manner. You want t make sure, that actions are executed only once, but also you want to be able to track if an action was executed at all or with errors.

# Some basic assumptions
a "Action" is a function to be called in an asynchronous manner together with its parameters. 

It should be assumed that an "action" can be made idempotent, meaning executing an action twice shoudl produce the same result - either by the function to be called is idempotent by itself or by just remembering the sucesful execution of the action at some leiable place

# Basics

# A Action is happening in Space and Time

