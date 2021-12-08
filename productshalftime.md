#### Notes on "Developing Products in Half the Time"

### Intro

- "For each month cut from a product's development cycle, up to a month is added to its sales life...The earlier a product appears, the better are its prospects for obtaining and retaining a large share of the market"
- "if a new product appears before there is competition, the company will enjoy more pricing freedom"
- "an ability to move quickly provides a great deal of flexibility. It can ebale you to get to market first, but it can also allow you to wait longer for the market or the technology to settle out before starting, still getting to market in time but with a better solution than the competition"
- Accelerated development means that companies will have to respond to customers needs rather than imitating competitors, which means they will defining the terms of the marketplace, forcing competitors to respond. See also OODA loops
- "most tools for accelerating development invove using resources more intensively through heavier staffing, and dedicating ample funds for quick prototyping. Roughly doubling the burn rate, and running it half as long."
- "much of the price of a faster development process shows up in a process that is in a sense messier. Different projects are organized differently, each to the needs for that particular projects. Decision making is more decentralized. This required more management attention and higher caliber people."
- "the only reliable way we have found to objectively assess the relative importance of cycle time is to do financial modeling to see how important a month of delay is financially"
- "even if rapid development is crucial to your business, you probably cannot afford to do it on every proejct. rapid development requires some of your most talented, enthusiastic individuals. Accelerated projects require priorities in service areas that may be difficult to provide to all projects. And fast projects require more management attention"
- "when management decides to develop a new product, two issues arise: deciding on the product to be developed, and deciding how development will be executed"
- "time to market is an excellent focal point around which to build an improved development system, as it tends to drive the basic changes in desirable directions: in order to get to market quickly, everything else must be working well. People from different departments must communicate effectively, non-value-adding activities must be eradicated, customers must be involved intimately, and management must be supportive"

### Putting a Price Tag on Time

- "speed is not the objective, it is a means to an end; the objective is making money"
- "four product development objectives: introduction date, unit cost, performance, and development expense. Each one trades off against the others"
- "only a small portion of the financial impact of being late to market shows up during the period of delay. The true impact is caused by the fact that you have shifted the timing of the sales ramp."

### The Fuzzy Front End

- "Each month of delay has a quantifiable cost of delay. Our goal as developers is to find opportunities to buy cycle time for less than this cost. These opportunities, large and small, appear throughout the development process. But there is one place we consistently find least expensive opportunities to achieve large improvements in time to market. We call this stage the Fuzzy Front End - it is the fuzzy zone between when the opportunity is known and when we mount a serious effort on the development project."
- "teh market clock measures the time it takes us to respond to opportunities in the marketplace. It starts ticking when a customer opportunity appears and continues inexorably ntil the customer's need is filled. Teh market clock is unforgiving. It keeps on ticking whether we are working on the project or not, and with each pssing minute we pay the cost of delay. The cost keeps accumulating steadily even when nobody is working on the project."
- "we should treat a week spent at the front end of a project with the same care that we would treat a week consumed at the very end."
- "Teh sense of urgency is lowest at the beginning of a product development, when tehre is no competition. but it is at this stage of lowest urgency when there is the greatest opportunity to cheap influence the project"
- "Make a person responsible for the front-end of the development cycle. By designating a specific individual responsible, you dramatically increase the chance that something will actually happen. Use someone who will later be a team member to maintain continuity between planning stages and execution"
- "capture new-product opportunities frequenly and early. This is done by making it easy to submit an idea, and by collecting and reviewing these ideas frequently. Most companies make it much too difficult to submit an idea. The objective of the idea-capture process is to achieve visibility, not to filter otu bad ideas. The filtering activity should occur after the idea is visible to management"
- "we can avoid developing technology inside of a project by creating technology assessment activities. Compaq did this well in the early stages of laptop computers. They were not the first to develop a laptop, but they monitored the major components needed against their pre-established criteria. When displays, hard drives, etc. reached teh threshold of maturity, they were prepared to jump into the market quickly."


### The Power of Pitfals of Incremental Innovation

- "The hardest way to achieve rapid development is to accomplish development tasks faster. The easiest way is to minimize the work required to develop the product"
- "Incremental innovation should be done as a two-step process: introduce new technology in a low-risk way, such as a low-volume product. Once issues with manufacturing, design, cost, and performance have been worked out in the low-risk situation, it can be scaled up to the higher volume application"
- "it is generally faster to adopt new technology using a two-step rocess because you waste little time optimizing the first step. You optimize during the second step when you really know what needs to be optimized. use the experience of the first step to guide the optimization during the second step."
- "either you put your own products out of business, or your competitors will do it for you"
- "there was no incremental path between steam and diesel railroads, or between vacuum tubes and transistors. There is an ultimate danger to the company that relies exclusively on incremental innovation, becasue eventually new technology will put it out of business"
- "consider the case of PARC - a research center that constantly generated new technology that never made its way into xerox's products. The main reason was the scientists were never transferred along with the technology. Bidirectional flow between product development and advanced technology (R&D) is important to achieve effective development"

### Capturing Customer Needs

- "a specification is an attempt to capture customer needs, which must start with the customer"
 - Who is the target customer
 - what is the customer's problem
 - how will the product solve this problem
 - which customer needs will this product not satisfy
 - which benefits will it offer compared with other solutions that are available to the customer
 - how will the customer value these benefits
 - on what basis will the customer judge the product?
- The specification should also circumscribe the scope of the project by delineating what the product will not do.
- If sales thinks it has enough features, that means it has too many features at the expense of cycle time
- Bulk of the customer contact should occur before design starts. If the customer is not involved before early decisions are made, momentum will prevent them from being reversed.
- Designers must be in direct contact with the customers so they can understand the context in which it will be used.
- customers buy benefits, not features
- People tend to write about what they can understand and describe. But the factors most likely to delay a product are the ones nobody understands, which seldom are written into the spec.

### Using System Design to Compress Schedules

- It is almost impossible for a subsystem designer to compensate for a major defect in architecture. In contrast, a good architecture can easily compensate for major defects in subsystem design.
- Five key architectural decisions
 - Where to draw the boundary between teh system and the rest of the world
 - how modular to make it
 - the interface between subsystems
 - how to maintain flexibility within the system
- Changes to the system boundary will change the use of the product, which will require reevaluating the requirements
 - example: a cordless shaver could be accidently activated inside luggage, and need a locking off switch. A plug-in shaver doesn't need this feature.
- Modularity allows for more concurrent development, decreased cycle time. But it adds cost and decreases performance
- interfaces are generally the weak link in the system, and a frequent source of failure
- Fast development requires locating functions so they don't cross module boundaries
- First key principle of interface design is to keep them stable. Nothing destroys the motivation to work harder than seeing nearly completed work made useless because the requirements changed. Avoid if possible (see: normal project development, architects)
- Make interfaces robust (generous margins of capability, etc.). More expensive, act as insurance against design changes/mistakes
- you don't need to know exactly what customers want as long as the architecture is flexibile enough to meet their needs. Flexibility adds cost, but allows for reduced cycle time.
- concentrate risk in one portion rather than spreading it amongst many modules. Increases likelihood of success, simplifies management, most talented people can be allocated to those modules
- system integration risk: is the risk that modules will not work together. Creates great schedule risk because it occurs on the critical path, near the end of development.
 - can be reduced by concentrating risk in one module and with robust interface design
- companies tend to ship their org charts

### The Team Leader / Building the team

- no decision more critical to product success than choosing a team leader
- team leader not technical role; they are peopel who can view it as a business proposition
 - but best team leaders have technical background. Allows credibility with engineering team and make better design judgments.
 - can be risky to have technical expert, as they will get drawn into technical minutiae
- leader should have clear vision of customer requirements, and competitor product offerings
- rule of thumb for product meetings: everyone should leave with action items. If you have no action items, you're deadweight on the project.
- activities most likely to delay project are those of part-timers who have other project work. Thus the part time staff need the most management to prevent delays on the critical path. Assume the less work someone has to do, the more likely they are to create a delay.
- higher levels of dedication require smaller teams, thus reducing communication overhead. And more dedicated staff will have higher level of commitment.
- teams should be organized around the physical or logical subsystems of the product
- certain early activities help the team to gel quickly. Begin by giving them a clear, challenging, and important objective
 - discuss and agree on work process
 - create product spec, product schedule
 - assess risk areas of project

### Organizing for Communication 
- developing a new product entails making thousands of decisions, and weak communication can delay these decisions or yield poor decisions that result in unnecessary design rework. The delay may seem minor, perhaps a day or a few hours, but the aggregate effect of delaying thousands of decisions is staggering. If project decisions are not made by the peopel working in the project daily, the project can be delayed every time such a decisino is needed. Consequently, our team design strategy is to minimize the need for external communication by giving the team teh resources and authority to make the vast majority of project decisions itself. Appropriate organization and delegation of decisions avoids many of these delays.
- trade off between managers that manage functional/regional areas, and team leaders that lead cross functional teams. trade off between relative amounts of authority.
- best might be heavyweight team leader, where team leader controls all project related issues, but people continue to be under their functional manager. When project is over, people return to their managers
- research suggests a team of 5 to 8 works most effectively
- an underlying concern is that people will not be kept busy. In practice this is not an issue - people generally plan ahead to keep work off the critical bath
- in many companies, colocation credited for shortening development cycles
 - toyota has seven times face to face contact with supplier engineers than its rivals; credits this with advantages in cycle time, productivity

### Designing a fast development process
- experts at development keenly aware of which activities are on the critical path, and strive to constantly remove them from critical path
- basic tool of rapid development is overlapping: working on many activities concurrently

### Controlling the process
- When reacting is less expensive than forecasting, it makes business sense to react
- must deploy most talented people to the cross functional teams to achieve rapid development
- Should have both a system of formal reviews and frequent, informal product reviews. When reviews are frequent they catch design problems before they can solidify and require extensive rework
- fastest method of development is when an engineer can be dedicated full-time to a project
- most effective way of staffing: rank projects in order of importance. Then go down the list, and assign as many people as can be effectively engaged. Then move on to the next project, etc.
- when a product first hits manufacturing, we learn a lot about its limitations very quickly, and fix issues quickly. Some rework on a design is healthy because it is a sign that we are making trade-offs between engineering time and manufacturing rework - a design that has no changes after release to manufacturing probably spent too much time in design
- make it easy to reuse parts
- role needed early in the project is more a leader than a manager; showing the vision and preparing staff for it, setting expectations, etc.
- key things to have:
 - an accountable, committed team
 - a team with sufficient authority and resources to get the job done
 - a clear, stable direction
- what usually impedes organization is not its structure, which can be redesigned, but its udnerllying values, which cant