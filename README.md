# SparkPost Data Engineering Take Home Project

The purpose of this project is for you to be able to demonstrate your ability to use Spark to process data. There is no single "correct" way to complete this project. You should only need to set aside 2-3 hours to complete this project. 

## Data Sources

* /data/customers/: A list of customers and their active status
* /data/mailbox-providers/: A list of routing domains what mailbox provider they use
* /data/events/: A set of events

## Problem Statement

Using Spark, create a script that will process a single day of event data and output data in with the following criterion: 

* The output shows the number of injection events sent by each customer to Verizon Media routing domains each day
* Only process data for active customers
* The data should be partitioned by day
* Output exactly 1 file per day

#### Extra Credit (if time allows):

* Add a configurable threshold value that can be used to exclude traffic below a certain volume
* Include all mailbox providers, not just Verizon Media
* Add the percentage of traffic sent to each provider
