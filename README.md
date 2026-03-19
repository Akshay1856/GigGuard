# DevTrails
**Requirement Detail:**

Scenario 1: Environmental Issue
1. Heavy rains hit a part of chennai and the roads are under a foot of water. Naturally, it is too dangerous for a bike to pass through. Considering the rider misses around 5 hours of work during the busy dinner time, we make sure that the software notes the rainfall data for that specific pincode and pays the rider for those hours automatically.

Scenario 2: Social Issue
3. Let us consider a sudden VIP visit or a road block due to construction in the prime areas of the city. The rider is essentially working but cannot reach any restaurants or the customers in the said zone. Our system detects the zone through data and triggers a payout for the lost time.

**Application Workflow:**
1. Sign-up: The workers register via a mobile app and authenticate their ID.
2. Profiling: Assigning a risk weight based on the location.
3. Weekly-Plan: This Weekly Premium model is so that it aligns with the weekly payout cycles.
4. Parametric trigger: When the threshold is breached, we make sure to validate the workers online status. Once confimed, the system calculates the wage based on past data average and makes an automatic transfer.

**Weekly Premium Model:**
We have structured our financial model on a Weekly basis to align with how food delivery partners in Chennai receive their payouts.
1. Instead of a heavy monthly cost, the rider pays a small subscription fee, for example: ₹25–₹40 every Monday. The cost is recalculated every week based on upcoming data.
2. If a rider works in a flood-prone area, it is  made sure that the system adjusts slightly to reflect the higher chance of a payout.
3. The small fee ensures that the rider never feels financial burden considering the high amount they might have to pay on a monthly basis.

**Parametric Triggers:**
The platform is made to make sure that the rider is not made to file a claim and the system triggers itself based on data.
1. Intense Rainfall: A payout is automatically triggered when rain exceeds 30mm within a 60-minute period, identifying conditions where road navigation becomes unsafe.
2. Extreme Heat: The system activates a heatwave claim when the Chennai Heat Index crosses 45°C, protecting riders who must stop working during peak afternoon hours for safety.
3. Social & Civil Disruption: We plan to utilize real-time traffic and news APIs to trigger coverage when a specific delivery zone is blocked due to unplanned strikes or political rallies.
4. Platform Technical Failure: In the event of a major delivery app server crash lasting longer than 45 minutes, our platform compensates for the lost earning window during that period.
5. Strict Coverage Scope: All triggers are exclusively designed to cover lost income and strictly exclude health insurance, life insurance, or vehicle repair costs.

**Mobile App:**
We have chosen a Mobile Application because it allows us to use GPS to verify that a rider was actually present in a disrupted area during a trigger event.
1. Fraud Prevention: A mobile platform enables device fingerprinting and helps detect spoofing which is essential for preventing duplicate or fake claims.
2. Instant Accessibility: Since most food delivery partners rely on smartphones for their daily tasks, a mobile app provides the most seamless user experience for receiving an automatic payout notifications.
