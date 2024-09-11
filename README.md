# Restaurant-Simulation
Self Project

A Java program for event-based simulation of the billing counter of a burger restaurant (McMohan's Burger)

**Goal:**
We want to develop a simulation system for a big and famous burger restaurant called McMahon's Burgers, which gets a lot of customers leading to long billing and food preparation queues. We would like to know some statistics like average waiting time, average queue length, etc., so that proper steps to improve customer convenience can be taken.

**Description**

Customers arrive randomly and are automatically assigned contiguous integer IDs, starting from 1
A new customer always joins the billing queue with the smallest length at that time (If there are multiple billing queues with the same smallest lengths, then the lowest numbered queue of those is chosen by the customer)
If two customers arrive at the same time, one of them joins the queue first, then the next one joins (We need to decide whom to add first)
The billing specialist on the billing counter k will take k units of time to complete the order
After the order is completed, the customer order is printed automatically and sent to the chef, who prepares the burgers in the sequence he receives them
If two orders arrive simultaneously then the chef chooses the order from the higher-numbered billing queue first
The chef has a large griddle on which at most M burger patties can be cooked simultaneously
Each burger patty gets cooked in exactly 10 units of time
Whenever a patty is cooked another patty can start cooking in that instant
Upon cooking, the burger is delivered to the customer in 1 unit of time
Whenever a customer gets all their burgers, they leave the restaurant instantaneously (it’s a take-away restaurant with no dine-in)
