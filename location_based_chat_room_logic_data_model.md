# Location Based Chat Room

## Entity-Relationship Model
- All entity has identifier without physical meaning.
- Relationship will be joined by relationship table, in other word, entity itself does not contain relationship. 
- All data elements are immutable.

### Location
- Location can have many different types, we can the name only for the famous place. 
- Postal address should be able to be translated to geoLocation.

### User
- User may have an email address, s/he may choose to register the service which will give her/him more privilage. User can create one or many nickname for purpose of anonymous access. 

### ServiceRegistration
- register user and Service Level Agreement (SLA), in here, it is the privilige.

### Chat Room 
- Each chat room should a unique ID, It is an virtual location, which does not have to have physical location.
- User can create either a public or a private chat room. 

### Thread
- Each thread has its own unique attributes: subject, timeCreated, and status.
- There are many threads in a chat room. 

### Messages
- Each thread has many messsages. They are related to each other like a tree, but we will present this tree in a table of content manner. The latest message will be displayed at top; similar to Google email display.