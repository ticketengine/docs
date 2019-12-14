# Events
You can get an event up and running in Ticket Engine very quickly. There are 3 steps to create an event: 
1. Add basic event details
2. Create capacity
3. Create access

In more traditions ticketing solutions access might be called "tickets". But at Ticket Engine we chose access because it is more than just tickets. Some of your visitors might not need a ticket at all to enter an event. Maybe they are on the guest list or have some kind of membership that grands them entry. That's why we chose access as a concept over ticket.



## Details
In this tab you can mange the basic event details.

![alt text][event_details]

Field | Description
--- | ---
Name | Name of the event.
Description | Event description.
Time frame | Start and end of the event.
Tags | Event tags.

> NOTE: events can only be cancelled and rescheduled if no access have been issued yet.


## Capacity
In the capacity tab the inventory of access can be managed. The capacity consists of an Venue with one or more groups that define the available access. 
Groups can be used to allocate inventory to specific customers.  

![alt text][capacity_details]

Field | Description
--- | ---
Location | Name of the group.
Capacity | Total available inventory in the group.


## Access
The access tab is used to define one or more access types. An access type described where a customer has access to and under what conditions a customer can access the event.  

![alt text][accesss_details]

Field | Description
--- | ---
Name | Name of the access type.
Description | Description of the access type.
Access to locations | Capacity groups where customer should get access to. If more than one group is added the allocation strategy will issue access for the first group (in supplied order) where there is available capacity.
Use limit | The number of times access can be used at the door of the venue.
Tags | Access type tags. 
Conditions | The conditions a customer has to pass to be able te get access to an event.

### Conditions
The conditions consist of a tree of nested conditions. A customer has access to an event if he or she passes at least a single path in the condition tree successfully. 

Condition | Description
--- | ---
If | Add a new condition group.
Price | Defines the price a customer has to pay to be granted access.
Free entry | Customer does not have to pay to be granted access. 
Number of items in cart | 
Cart total value | 
Sales channel | The sales channel through which the order is placed.
Customer with tag |  
Birth date | Customers who's birth date is.
Current date | 


## Attendees
The attendee tab shows a list of all customers who have access to the event.


[event_details]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/event-detail-edit.png "Event details"
[capacity_details]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/event-capacity-edit.png "Capacity"
[accesss_details]: https://raw.githubusercontent.com/ticketengine/docs/master/assets/event-access-edit.png "Access type"
