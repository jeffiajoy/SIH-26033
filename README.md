# Smart India Hackathon Workshop
# Date: 24/11/2026
## Reference Number: 26003003
## Name: Jeffia Joy .T

## Problem Title
SIH 26033: Multiple intermediaries reduce farmers earnings and increase consumer prices.

## Problem Creater's Organization
Ministry of Consumer Affairs, Food & Public Distribution

## Theme
Agriculture, FoodTech & Rural Development

## Problem Description
Expected Solution: Create a digital marketplace that:

• Connects farmers/FPOs directly with consumers and bulk buyers.
• Provides logistics support.
• Uses AI for demand forecasting and route optimization.

Benefits:

• Better prices for farmers.
• Lower prices for consumers.
• Reduced supply chain inefficiencies.

## Proposed Solution
1. Detailed Explanation of the Proposed Solution
• KrishiSetu Direct (Proposed Platform Name): An AI-powered B2B and B2C digital agritech ecosystem that directly connects individual farmers and Farmer Producer Organizations (FPOs) with bulk buyers and retail consumer groups.
• Hub-and-Spoke Micro-Logistics: Integrates local third-party logistics (3PL) providers and idle rural transport (mini-trucks, tempos) to aggregate produce at village-level collection centers before dispatching to urban hubs.
2. How It Addresses the Problem
• Eliminates Middlemen: Replaces the traditional multi-tier mandi chain of village traders, commission agents, wholesalers, and retailers with a single transparent digital transaction.
• Solves Fragmented Supply: Enables small-scale farmers to pool their produce through FPOs to meet minimum order quantities required by bulk buyers.
• Reduces Transit Losses: Dynamic route optimization minimizes transit time for perishables, lowering post-harvest spoilage and transport costs.
3. Innovation and Uniqueness
• Dynamic Route & Load Pooling : Unlike standard delivery apps, our Vehicle Routing Problem (VRP) algorithm dynamically pools partial loads from multiple nearby farms onto a single shared vehicle, cutting per-kg freight costs by up to 30%.
• Vernacular Voice-First Onboarding: Allows farmers with low digital literacy to list produce, check live mandi benchmark prices, and accept bids via simple voice commands or WhatsApp/IVR bots in regional languages.
• AI-Assisted Quality Grading: Uses smartphone computer vision to instantly grade produce quality (size, color, blemishes), building trust with remote bulk buyers without needing physical inspection.

## Technical Approach
1. Technologies to Be Used
• Frontend: React Native (Farmer & Driver mobile apps with offline-first sync), Next.js (Bulk Buyer & FPO web dashboard).
• Backend & Database: Node.js / Express or FastAPI (Python), PostgreSQL with PostGIS (for geospatial queries), Redis (caching & real-time order matching).
• AI / ML Stack: Python, PyTorch / TensorFlow (CNN for visual crop grading), Prophet / XGBoost (time-series demand forecasting), Google OR-Tools (capacitated vehicle routing optimization).
• Integrations & Cloud: ONDC (Open Network for Digital Commerce) protocols, UPI / Escrow payment gateways, Bhashini API (vernacular voice translation), AWS / GCP.
2. Methodology and Process for Implementation
• Phase 1: Onboarding & KYC: Farmers/FPOs register via mobile/voice; bulk buyers verify GST/business credentials.
• Phase 2: Demand Forecasting & Listing: The AI engine analyzes historical consumption, weather, and festival calendars to publish weekly demand forecasts. Farmers list available harvest quantities and expected prices.
• Phase 3: Smart Matching & Escrow: Buyers place orders, funds are locked in a secure digital escrow account to guarantee payment upon delivery.
• Phase 4: Route Optimization & Dispatch: Google OR-Tools clusters nearby farm pickups and assigns the optimal vehicle route. Real-time GPS tracking updates buyers on ETA.
• Phase 5: Delivery & Instant Settlement: Upon QR-code scan at the buyer's doorstep, escrow automatically releases funds directly to the farmer’s bank account via UPI.
<img width="1774" height="887" alt="Food Supply Chain Flowchart" src="https://github.com/user-attachments/assets/2f0c1f2b-6c91-4795-925a-be317c62781b" />


## Feasibility and Viability
. Analysis of Feasibility
• Technical Feasibility: Built on proven open-source geospatial and ML frameworks, offline-first architecture ensures usability in low-connectivity rural areas.
• Operational Feasibility: Asset-light model—the platform does not buy trucks or warehouses, instead utilizing existing FPO collection centers and local 3PL fleet operators.
• Financial Viability: Sustainable revenue through a nominal 2–3% platform/logistics facilitation fee paid by bulk buyers, keeping the platform zero-commission for farmers.
2. Potential Challenges and Risks
• Digital Literacy & Trust Deficit: Farmers may hesitate to shift away from familiar local commission agents (arhatiyas) who offer instant cash.
• Quality Disputes: Disagreements between remote buyers and farmers regarding produce freshness upon arrival.
• Cold-Chain & Perishability: High spoilage risk for delicate fruits and vegetables during summer transit.
3. Strategies for Overcoming Challenges
• FPO Ambassadors & Instant Escrow Payouts: Partner with trusted local FPO leaders for onboarding and ensure instant T+0 bank settlement upon pickup/delivery to match cash liquidity.
• Standardized AI Grading + Pre-Dispatch Verification: Capture timestamped, AI-graded photos at the village pickup point to establish an indisputable quality baseline.
• Smart Perishability Routing: Prioritize perishable goods in the routing algorithm for early-morning/night transit and match them with available reefer (refrigerated) vehicles.


## Impact and Benefits
1. Target Audience Impact
• Small & Marginal Farmers : Gain transparent market access, fair price discovery, and guaranteed timely payments.
• Bulk Buyers : Secure consistent, traceable supply at wholesale rates without mandi markups.
• End Consumers: Access fresher produce at lower retail prices.
2. Multi-Dimensional Benefits
• Economic: Increases farmer net income by 15–25% by capturing middleman margins, while reducing end-consumer prices by 10–15%.
• Social: Empowers rural FPOs, reduces farmer distress caused by price volatility, and creates local gig-economy jobs for rural transport drivers.
• Environmental: AI route pooling reduces empty-truck miles and carbon emissions, demand-aligned harvesting cuts food waste and landfill methane.

## Research and References
• Platform & Problem Context: Details on problem statement requirements and landscape analysis via SIH 2026 Problem Portal and SIH Buddy.
• Government & Policy Frameworks: e-NAM (National Agriculture Market) for mandi price benchmarking and ONDC Agriculture Domain for interoperable network standards.
• Technical & Algorithmic Research: Google OR-Tools Vehicle Routing for multi-pickup route optimization and Bhashini AI for vernacular voice interfaces.
• Supply Chain Studies: Post-Harvest Losses in Indian Agriculture highlighting how direct farm-to-fork logistics can curb the transit wastage in fruits and vegetables.
