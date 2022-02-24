- Start Date:  (2022-02-23)
- Members: (Francisco Rojas [PFranciscoRojas] - Marlon Ramirez [malonr]) 
- RFC PR: (leave this empty)

# Summary
Architecture Database Design for Account User and selection of what Database we should use.

# Basic example


# Motivation

Why are we doing this?
We are doing a schema because users from our Booking need  to fill in their basic information and our booking system can storage that information.

What use cases does it support?
Huge and success systems have had a well organized schema and applied the CAP theorem to select what Database is necessary for their project.
 
What is the expected outcome?
Having users personal information organized in a schema will help us to build a well structured database. It also will help us to scalate our product easily. We also expected that the Database chose by us  is going to be enough to support the needs of  our booking system. 

# Detailed design

![image](https://user-images.githubusercontent.com/58435018/155622919-25f1a224-4233-4ca4-a104-d4c0c8d0a9d3.png)

After investigating how we should build our schema, Francisco built the schema above. We added new attributes to users such as: currency.


We decided our database should be CA (Consistensy and Availability) . First, Consistensy our users have to be able to  see the same data no matter which node they connect to on the system. Second, Availability because our users have to see their data whenever thay woudl like to. 

We decide to follow a relational BD due to we have identifiers in the previous schema that we allows to do a relation between tables, and we can use the SQL language for manipulating data. 

# Drawbacks


# Alternatives

What other designs have been considered? We could also apply Postgres as our database because is one of the option when chossing CA from the CAP theorem.  

What is the impact of not doing this? Without a user acount system other teams couldn't work properly without user's personal information such as : Marteking. 

# Adoption strategy

If we implement this proposal, how will existing C9 developers adopt it? Is
this a breaking change? Can we write a codemod? Should we coordinate with
other projects or libraries?

# How we teach this

What names and terminology work best for these concepts and why? 

Schema = Show database using graphics, this way make it easy to understand how is data organized without looking at the code. 

CAP theorem = The best proven way to select databases for projects. It gives you the exact answer of why you really need for your project (Consistency, Availability, Partition Tolerance)

How is this idea best presented? 
It could be present in a short meeting. One of us could explain it.

As a continuation of existing C9 projects patterns?

Would the acceptance of this proposal mean the C9 documentation must be re-organized or altered?
No, It would not. 

Does it change how C9 is taught to new developers at any level?


How should this feature be taught to existing C9 developers?

# Unresolved questions

We haven't compared MySQL to postgres
