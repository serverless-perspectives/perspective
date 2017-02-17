Future world
- Speed of idea to production increases, could drop to a single day, hour, minute
- Data analytics effort by ops shifts from uptime to business value metrics
- No more undifferentiated heavy lifting!
- All of this removes you from working in the bottom half of the value chain - leave that to the cloud providers

After teams have removed themselves from bottom half of value chains, what do they look like?
- Product owners are experimenters, hypothesizers, model-builders
    - Learn how to posit and validate results
- We don't know what exactly this enables but it can only be good
    - Remove scarcity of time and money
    - Analogous to other utility revolutions - bolts, electricity, etc.
- Chief constraint of business scalability no longer IT
    - Decoupled the lockstep pattern of IT buildout and business buildout
    - Decoupling IT speed/agility from ability to innovate

Concerns people might have about these claims
- This is too far in the Future
- Works for Netflix but too hard for companies like mine to achieve


The entire point of software development and IT is to enable, support, and provide business value.  Yet how much of the time and cost spent by IT adds direct value, and how much of it is undifferentiated heavy lifting?  Are you spending time managing servers?  Do you have a checklist for application and database deployments?  Is asking for a new dedicated environment akin to touching the third rail?  Are you spending time architecting and designing for application scalability?  Is the entire development, testing, and releasing process so expensive and restrictive that you bundle up months worth of work before finally committing a big-bang deployment through to production?  Are there multiple levels of change control and decision making required for even simple feature enhancements because the cost associated with making them necessitates formal cost control procedures?  None of that adds value to your customers - it's all undifferentiated heavy lifting.  Undifferentiated because it adds no value, it's not remotely core to your organization.  And heavy because it's not simple - it's incredibly complex and time consuming.  And because of the investment required it distorts decision making incentives and results in incredibly inefficient behaviors and practices within an organization.  How has the pace of IT resulted in practices (both for IT and business users) that would no longer apply in a world where the amount of time spent on undifferentiated heavy lifting is significantly reduced by orders of magnitude?

First let's talk about undifferentiated heavy lifting.  It's everything you have to do between someone having an idea and the idea being realized and put in front of customers that isn't directly related to that idea.  An example might be in order.

An energy company has a popular power contract platform for their internal and external sales team.  It provides them with the ability to manage and sell energy contracts that fit the needs of their customers - they can choose products that let them lock in at current prices, or they can ride the market.  Salespeople can establish margin thresholds they want to achieve.  They can manage all of their customers and prospects in a single system and keep track of when they are eligible for renewal.  They can email contracts from the app, print it off, have the customer sign, take a picture, and  then upload the contract - all within the app.

The natural gas sales team has a similar app.   It also has a feature that the power team would like to add - a sweet spot graph.  It's a graphical component that let's salespeople show customers prices that they could sign up for under different products and contract lengths.  It's a simple and intuitive tool that gives customers confidence that they are getting the best rate possible by being able to compare all their options in an easily-digestible and interactive graph.

That's the idea - add a sweet spot graph to the power platform.  What's it going to take to provide this feature for power customers?

Releasing the code to production is a manual and tedious process.  As a consequence deployments of disparate functionality is frequently bundled together in an attempt to save time.  The natural outcome of this is that deployments are riskier - many unrelated changes are being grouped together.  Not only does this increase the likelihood of defects or unintended consequences, it also makes tracking down the root cause of the issues harder and more time consuming.  Because of this the deployments typically happen at times the application isn't being heavily used - in this case late at night on a Friday, which provides weekend time for resolving issues but also means all teams involved with the deployment have set aside a weekend.  Let's say that the earliest release that can accommodate this change is at least a month out - which is 