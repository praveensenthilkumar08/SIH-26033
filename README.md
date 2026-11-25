Smart India Hackathon Workshop
Date: 24 November 2026
Reference Number: 26000307
Name: Praveen S

Problem Title
SIH 26033: Multiple intermediaries reduce farmers' earnings and increase consumer prices.

Problem Creator's Organization
Ministry of Consumer Affairs, Food & Public Distribution

Theme
Agriculture, FoodTech & Rural Development

Problem Description
Expected Solution: A digital marketplace that connects farmers/FPOs directly with consumers and bulk buyers, provides logistics support, and uses AI for demand forecasting and route optimization.

Benefits: Better prices for farmers, lower prices for consumers, and reduced supply chain inefficiencies.

Proposed Solution
UzhavuSetu: A Pre-Order Based Farm-to-Institution Vegetable Marketplace for Tamil Nadu

1. Detailed explanation of the proposed solution

UzhavuSetu ("Uzhavu" means farming in Tamil) connects FPOs and small vegetable farmers around Chennai (starting with the Chengalpattu and Kancheepuram belt) directly with hostels, college canteens, hotels and apartment communities. Instead of farmers harvesting first and searching for a buyer later, the platform works on a "sell before you harvest" model.

Demand-locked harvest: Buyers place pre-orders or weekly subscriptions 2 to 3 days before harvest. Orders are pooled, and farmers harvest only what has already been sold. This reduces unsold produce and forced distress sales.
Voice-first Tamil app and WhatsApp bot: Farmers or FPO coordinators list crop, quantity and harvest date by speaking in Tamil. No typing or English is needed.
AI Price Advisor: Suggests a fair price band by comparing recent mandi prices (Agmarknet/e-NAM), weather and local demand, so farmers don't depend on an agent's quote.
AI demand forecasting: Learns each buyer's weekly pattern (for example a hostel's daily vegetable needs) and tells FPOs what to plant and supply.
Hub-based pooled logistics: Existing FPO centres, cooperative shops and Uzhavar Sandhai (farmers' market) spaces act as collection hubs. A route optimizer pools pickups from several farms into one vehicle and one delivery run, which lowers cost per kg.
Rupee Trail bill: Every order shows a simple bill: what the farmer gets, transport cost, platform fee and what the buyer pays.
Escrow payment: The buyer pays by UPI into escrow, and the farmer is paid after delivery confirmation, targeted within 24 to 48 hours.
AI quality check: The farmer uploads a photo, and the app grades size, colour and visible defects so buyers can trust quality without a middleman.
2. How it addresses the problem

Problem	UzhavuSetu solution
Many intermediaries add margins	Direct farmer-to-buyer ordering with a small, visible platform fee
Farmers don't know fair prices	AI Price Advisor using live mandi data
Unsold produce and price crashes	Pre-orders and demand forecasting match supply to demand
High transport cost and spoilage	Pooled pickups, local hubs, optimized routes
Consumers pay inflated prices	Fewer layers means a lower final price and fresher produce
Delayed payments to farmers	Escrow with fast release after delivery
3. Innovation and uniqueness

Sell-before-harvest model that guarantees demand rather than just listing produce
Rupee Trail bill that makes margins visible on every order
Existing hubs reused (FPO centres, cooperatives, Uzhavar Sandhai) instead of building new infrastructure
Tamil voice-first design for farmers with low digital literacy
Focus on institutional buyers (hostels, canteens, apartments) whose demand is regular and predictable
Works alongside e-NAM and Agmarknet by using their data instead of competing
Technical Approach
1. Technologies to be used

Layer	Technology
Frontend	React Native (mobile), React (web), WhatsApp Business bot
Backend	Python (FastAPI), PostgreSQL, Redis
AI/ML	XGBoost/LSTM for price and demand forecasting; CNN (MobileNet-based) for produce grading; Bhashini APIs for Tamil speech-to-text and translation
Data sources	Agmarknet/e-NAM prices, IMD weather data
Logistics	Google OR-Tools for route pooling, Google Maps API, GPS tracking
Payments	UPI with escrow-style hold and release
Traceability (optional)	QR code on each batch showing farm, harvest date and delivery
Cloud	AWS/Azure/GCP with offline-first caching for weak rural networks
2. Methodology and process for implementation

System flow:

Buyer (hostel/canteen/apartment) places pre-order or weekly subscription
                    ↓
Orders pooled by crop, area and delivery day
                    ↓
AI forecasts demand + suggests fair price band
                    ↓
FPO/farmer accepts order by voice (Tamil) → harvests only what is sold
                    ↓
Farmer uploads photo → AI quality grade
                    ↓
Optimizer pools pickups → village hub → single delivery route
                    ↓
Delivery → Buyer confirms → Escrow released to farmer
                    ↓
Rupee Trail bill generated → Ratings exchanged
Implementation plan:

Phase	Timeline	Activities
1	Months 1 to 2	Interviews with farmers, FPOs and hostel/canteen managers; UI/UX design
2	Months 3 to 4	Build core app: pre-orders, listing, escrow payment, Rupee Trail bill
3	Months 5 to 6	Add AI price advisor, demand forecasting, quality grading, route pooling
4	Months 7 to 8	Pilot with 1 FPO and 2 to 3 vegetables (e.g., tomato, brinjal, lady's finger) serving a few Chennai hostels/canteens
5	After pilot	Measure results, refine, extend to more crops and districts
Prototype / screenshots: [Insert your prototype link or screenshots here]

Feasibility and Viability
1. Analysis of the feasibility

Technical: Built on proven tools and open government data (Agmarknet, e-NAM, IMD, Bhashini).
Operational: Starts small with one FPO, a few crops and a handful of institutional buyers in one city.
Economic: Revenue from a small transaction fee (target around 3%, to be validated in the pilot), a margin on pooled delivery, and subscriptions from institutional buyers.
Policy fit: Aligns with Digital India, e-NAM, the FPO scheme and Agri-Stack.
2. Potential challenges and risks

Low digital literacy among farmers
Farmers' trust in a new platform and in payment timing
Spoilage during transport
Poor rural internet connectivity
Buyers' habit of using local suppliers
Resistance from existing middlemen
3. Strategies for overcoming these challenges

Challenge	Strategy
Low digital literacy	Tamil voice interface and WhatsApp bot; village "Kisan Mitra" helpers
Trust	Escrow payments, ratings, working through FPOs farmers already trust
Spoilage	Short harvest-to-delivery window, nearby hubs, pooled routes, cold storage tie-ups where available
Connectivity	Offline-first app with SMS/IVR fallback
Buyer adoption	Weekly subscriptions with consistent quality and a clear price bill
Middleman resistance	Give them roles as hub operators and delivery partners
Impact and Benefits
1. Potential impact on the target audience

Farmers/FPOs: A larger share of the final price, assured demand before harvest, faster payment, and less dependence on agents
Institutional buyers and consumers: Fresher vegetables, lower prices, steady supply and clear pricing
Rural communities: New work as hub operators, graders and delivery partners
2. Benefits of the solution

Social: Gives small farmers fair market access and a voice in their own language
Economic: Better farmer income, lower buyer cost, fewer supply chain inefficiencies
Environmental: Less postharvest waste because farmers harvest only what is sold, and fewer transport trips through pooling
Pilot success metrics: Farmer price per kg compared with mandi price, buyer cost compared with retail, spoilage percentage, payment settlement time, and number of repeat buyers.

Research and References
Agmarknet: https://agmarknet.gov.in
e-NAM (National Agriculture Market): https://enam.gov.in
Bhashini (Government of India language AI): https://bhashini.gov.in
India Meteorological Department: https://mausam.imd.gov.in
Google OR-Tools: https://developers.google.com/optimization
Ministry of Agriculture & Farmers Welfare and NITI Aayog publications on agricultural marketing reforms
[Add your own field notes: e.g., "Interview with FPO/farmer at ___, date ___"]
