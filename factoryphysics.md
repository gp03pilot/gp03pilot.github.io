Chapter 1

-Manufacturing employed as much as 40 percent of the U.S workforce in the 1940s, but less than 13 percent by 2006.

-factory physics broken down into "basics", "intuition", and "sythensis"
	-basics: the language and elementary concepts for describing manufacturing systems (variability, reliability, queuing systems, etc)
	-Intuition: single most important skill of manufacturing manager, intiution about the behavior of manufacturing systems
	-Synthesis: ability to bring disparate components of a system into an effective whole

-[Picture of the product process matrix]

-manufacturing environments vary greatly with respect to their process structure, the way material moves through the plan. Process structures broadly are:
	-Job shops: small lots produced with a high variety of routings. Flow through the plan is jumpled, and setups are common
	-Disconnected flow lines. Product batches are producted on a limited number of routings. routings are distinct, but there's no paced material handling system, so inventories build up between stations. Most manufacturing falls into this category
	-Connected flow lines: the classic moving assembly lines. Product is fabricated and assembled along a rigid routing.
	-continuous flow processes: continuous product (food, chemicals, oil, roofing material) flows automatically down a fixed routings. Suitable for extremely uniform products

-higher volumes = smoother flow structures. Thus, the manufacturing environment is dependent the stage in teh product lifecycle. Challenge of modern manufacturing is how to structure the environment so it attains the speed and low cost of high volume flow lines while retaining the flexibility and customization potential of a low volume job shop.

-Primary perspective of this book is discrete parts production on disconnected flow lines

-Circa 1988, there were 10 lawyers to every 1 engineer in the US, and 10 engineers to everyr 1 lawyer in japan

-In american industrial engineering, setup times were regarded as constraints, leading to the development of complex mathematical models for determining optimal lot sizes that would balance setup costs vs inventory carrying costs. In contrast, japanese focused on use of jibs, fixtures, etc to reduce setup times, resuling in "single minute exchange of die", allowing japanese plants to be the most productive in the world.

-"even with the availability of coal, large-scale production facilities did not immediately arise. The modern integrated industrial interprise was not the consequence of the technological and energy innovations of the first industrial revolution. The mass production characteristic of larage-scale manufacturing required coordination fo a mass distribution system to facilitate the flow of materials and goods through the economy. The second industrial revolution was catalyzed by innovations in transportation and communication - railroad, steamship, and telegraph - that occured between 1850 and 1880"

"Railroads were the spark that ignited the second industrial revolution for three reasons:
	They were america's first big business, so the first place where large scale management and accounting practices were needed
	Their construction (along with the telegraph system) created a market for mass-produced products
	they connected the country, creating mass-markets"

-"Sears and roebuck sales grew from $138,000 in 1891 to 37,000,000 in 1905"

-'In europe and japan, goods were sold to populations in established centers with strong word-of-mouth contacts. Advertising was largely a luxury. Advertising/marketting was more iimportant in the new world than the old.'

-"in 1868, america was still a minor player in steel, producing only 8500 tons to britain's 110,000...by 1879, it nearly equaled that of britain. And by 1902, america produced 9,138,000 tons to britain's 1,826,000"

-"cargengie's steel mill wasthe first steel mill whose layout was dictated by material flow. By relentlessly exploiting scale advantage and increasing velocity of throughput, carnegie quickly became the most efficient steel producer in the world."

-"in the 1870's iron rails cost $100 per ton. By the late 1890's they sold for $12 per ton"

-'ford's insight was to take the work to the man, not hte man to the work. Assembly lines just one of the techniques used for ths'

"in 1945 the american market was 8 times the size of the next-largest market in teh world, giving american firms a huge scale advantage. American per capital income 8 times that of japan in the 1950's, providing a vast source of capital...labor productivity was double that of any european countryk, 3 times that of germany, and 7 times that of japan. America could produce and distribute goods at a pace and scale unthinkable to anyone else."

Chapter 2 - Inventory Control

The economic order quantity (EOQ) model recognizes the idea that there is a tradeoff between lot-size and inventory. Increasing the lot size increases the average amount of inventory on hand (and holding inventory has costs), but reduces the frequency of ordering (which also has costs)

EOQ model also shows that the sum of holding and setup costs is fairly insensitive to lot size [show craph on page 54 here]

EOQ assumes instantaneous production - a model extended to an actual production time is the economic production lot (EPL) model

Wagner-Whitin algorithm for optimal production scheduling

Various statistical inventory models:

News vendor model of EOQ - Single replenishment, only issue is to determine order quantity in face of uncertain demand (ie: newspapers which are printed at the beginning of the day, sold a random amount, and discarded at the end of the day)

basic insights:
	-in an environment of uncertain demand, the appropriate production or order quantity depends on both the distribution of demand and the relative costs of overproducing vs underproducing
	-if demand is normally distributed, then increasing the mean demand increases the optimal order quantity.
	-if demand is normally distributed, then increasing the variability of demand increases the optimal order quantity if cs/(cs + c0) > 0.5, and decreases it if cs/(cs + c0) < 0.5 (cs = cost per unit of shortage, c0 = cost per unit of overage)

Base stock model - Inventory is replenished one unit at a time as random demands occur, so only issue is to determine reorder point.

Base stock can be used to control work release in multistage production. Base stock is established at each workstation; whenever an item is removed from the buffer, a replenishment order is triggered. This is essentially what kanban does.

insights from base stock model:
	-reorder points control the probability of stockouts by establishing safety stock.
	-the required base stock level (and hence safety stock) that achieves a given fill rate is an increasing function of the mean and (privided that unit backorder cost exceeds unit holding cost) standard deviation of the demand during replenishment lead time.
	-the "optimal" fill rate is an increasing function of the backorder cost and a decreasing function of the holding cost. hence, if we fix the holding cost, we can use either a service constraint or a backorder cost to determine the appropirate base stock level.
	-base stock levels in multistage production systems are very similar to card counts in kanban systems.

(Q, r) model - when inventory levels reach r, an order of size Q is placed. After a lead time of l, the order is received. Problem is to determien the values of Q and r. if Q is large, the part is replenished infrequently in large batches, then the stock level seldom reacehs the reorder point. If Q is small, then stock level frequently falls to hte rorder point and therefore has a greater chance of stocking out.

basic insights:
	-cycle stock increases as replenishment frequency decreases.
	-safety stock provides a buffer against stockouts.
	-(Q,r) model with a Q of 1 is the base stock model.
	-increasing the average annual demand D tends to increase the optimal order quantity Q
	-increasing the average demand during a replemnishment lead time increases the optimal reorder point r. This imiplies that either high demand or long replenishment lead times require more inventory for protection.
	-increasing the variability of teh demand process tends to increase the optimal reorder point. A highly variable demand process requires more safety stock than a very stable process.
	-increasing the holding cost h tends to decrease both the optimal replenishment quantity Q and reorder point r. (the more expensive it is to hold inventory, the lesswe should hold),

(Q, r) model offers general insights and practical tools, and is a very important model.

Overall inventory control insights:
-there is a trade-off between setups and inventory. (the more frequently we replenish inventory, the less cycle stock we will carry)
-There is a trade-off between customer service and inventory (higher customer services levels require higher levels of safety stock)
-There is a trade-off between variability and inventory

[put inventory model classification here]

----------------------------------------

Chapter 3 - material requirements planning (MRP)

MRP works by working backward from a production schedule of an independent-demand item to derive schedules for dependend-demand item. It's a push system, in contrast to a pull system like kanban, which authorizes production as inventory is consumed. the main focus of MRP is on scheduling jobs and purchase orders to satsify material requirements for a production schedule.

The four basic steps of MRP are netting (computing net demand), lot sizing (scheduling production quantities), time phasing (determining when to produce), and BOM explosion (breaking down the BOM into individual quantities)

Nervousness (ie: lack of robustness) in MRP occurs when a small change in the production schedule results in a larage change in teh planned order releses.

MRP II = manufacturing resources planning

Job dispatching = develop a rule for arranging the queue in front of each workstation that will maintain due date integrity while keeping machine utilization high and manufacturing times low. Over 100 different dispatching rules, but only way to consistently achieve godo schedules is to consider the shop as a whole.

----------------------------------------

Chapter 4 - Lean/JIT

"Just-in-time flow requires a very smoothly operating system. if materials are not available when a workstation requires them, the entire system may be disrupted. This has serious implications for the production environment. One means for avoiding disruptions is ohnos concept of autonomation, which refers to machines that are both automated, so that one worker can operate many machines, and foolproofed, so that they automatically detect problems."

The seven zeros which are required to acheive zero inventories:
-Zero defects:
-zero (excess) lot size: goal is a lot size of one
-zero setups
-zero breakdowns
-zero handling
-zero lead tiem
-zero surging (smooth production flow without changes)

"five whys"

kanban best suited to a repetitive manufacturing environment

Key to setup reduction is the distinction between internal setup and external setup. Internal setup operations are those tasks that take place when the machine is stopped. External setups can be completed while the machine is running. Four concepts for setup reduction:

1. Separate the internal setup from the external setup.
2. Convert as much as possible of the internal setup to the external setup
3. Eliminate the adjustment process with jigs, fixtures etc.
4. Abolish teh setup itself.

JIT best served by cross-trained workers who can move where needed to maintain the flow. Aided by machines arranged in a "u" so workers can easily monitor multiple machines.

analogy of water in a stream with rocks on the bottom. Water represents WIP, rocks represent problems. A high level of water hides the rocks; when the water level is lowered, the rocks are exposed. When WIP is reduced, problems and defects become noticeable.

Seven principles of quality from JIT:

1. Process control - make sure production processes are operating correctly.
2. easy-to-see quality - visual displays, boards, gauges, meters etc.
3. Insistence on compliance at every level
4. Line stop - each worker given authority to stop the line
5. Correcting one's own errors, giving workers full responsibility for quality.
6. 100 percent check - goal of inspecting every part, not just a random sample
7. Continual improvement

push vs pull production control systems: in a push system, such as MRP work releases are scheduled. In a pull system, work releases are authorized. A push system accommodates due daets, but has to be forced to respond to changes in teh plant. A pull system responds directlly to plant changes, but must be forced to accomodate customer due date (by matching a level production plan against demand)

Lessons of JIT/Lean and Six Sigma:
1. The production environment itself is a control - strategies that involve reducing setups, changing product designs with manufacturing in mind etc. have great impact.
2. Operational details matter strategically - small production details can give a substantial competitive advantage.
3. Controlling WIP is important
4. Flexibility is an asset
5. Quality can come first
6. Continual improvement is a condition for survival

and 

1. Quality and logistics must be improved together.
2. "if you don't have time to do it right, when will you ahve time to do it over?"
3. Variability must be identified and reduced

Chapter 5 - what went wrong?

value stream mapping - starts by making a "current state map" that identifies a characateristic flow of parts through the plan and then compares the "value-added" time with the toal cycle time of the part. The results are often stunning,k with value-added time being elss than 1 percent of hte total.

Chapter 6 - A science of manufacturing

production system involves 2 elements; demand and transformation. Essence is to trasnform material or other resources into goods/services to meet a demand.

Buffer: excess resource that corrects for misaligned demand and transformation. can take one of three forms:
	Inventory
	Time
	Capacity
variability: what makes alignment of demand and transformation impossible in practice

flow: material moving through a transformation process
stock: material waiting for transformation

mission statement: how the fundamental objective will be obtained on the strategic level

[hierarchical objectives in maufacturing goes here]
