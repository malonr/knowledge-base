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



This is the bulk of the RFC. Explain the design in enough detail for somebody
familiar with React to understand, and for somebody familiar with the
implementation to implement. This should get into specifics and corner-cases,
and include examples of how the feature is used. Any new terminology should be
defined here.

# Drawbacks

Why should we *not* do this? Please consider:

- implementation cost, both in term of code size and complexity
- whether the proposed feature can be implemented in user space
- the impact on teaching people React
- integration of this feature with other existing and planned features
- cost of migrating existing React applications (is it a breaking change?)

There are tradeoffs to choosing any path. Attempt to identify them here.

# Alternatives

What other designs have been considered? 

What is the impact of not doing this?

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


Optional, but suggested for first drafts. What parts of the design are still
TBD?