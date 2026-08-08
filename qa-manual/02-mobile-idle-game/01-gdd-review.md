# GDD Review

Review of the provided Game Design Document fragment for a mobile idle / city-builder game (details anonymized).

### Identified Ambiguities & Recommendations

| # | GDD Fragment | Problem / Ambiguity | Recommendation |
|---|--------------|---------------------|----------------|
| 1 | Parking → Queue | It is not specified whether there is a limit on the number of cars in the queue before the entrance | Clarify the maximum queue length or state that the queue is unlimited |
| 2 | Parking → Entry / Exit | Delay time or animation for these actions is not described | Add timing parameters (e.g. entry takes 2 seconds) |
| 3 | Upgrade → Effect | It is stated that an upgrade increases income, but it is unclear whether effects stack | Clarify whether new upgrade effects are added, multiplied, or replace the previous one |
| 4 | Cash Desks → Overloaded desk | It is unclear how quickly an NPC goes to departure and whether it can return if a spot becomes free | Specify whether the NPC disappears immediately or waits; whether it can rejoin the queue |
| 5 | Cash Desks → Upgrade button | It is written that money “is not deducted”, which looks unusual and may be an error | Clarify the logic: should the upgrade really be free? This seems inconsistent |
| 6 | Buildings → Autonomous work | Start condition is not specified: does the building start working immediately or does it need activation | Clarify whether any action (click, timer, etc.) is required to start the building |
| 7 | Helicopter / Rewarded ads | Behavior is not described when the video is unavailable or fails to play | Add fallback logic (retry option or user message) |
| 8 | Returning to the game (Offline) | Offline income calculation is not described — fixed rate or time-based? | Provide a formula or example of how offline income is calculated |
| 9 | Station → N seconds | “N seconds” is mentioned, but it is unclear whether this value can be changed in the game | Specify whether the value is constant or can be modified (e.g. by upgrades) |
| 10 | Overall structure | Some terms are duplicated or inconsistent (“bills”, “income”, “income from slot”) | Unify parameter names throughout the document to avoid confusion |

---

### Core Game Loop

1. **Income generation**  
   Player receives currency from parking slots, cafes and cash desks. Resources accumulate in real time, including while offline.

2. **Parking & NPC management**  
   Cars enter parking and generate income. NPCs move through queues to cash desks, complete payment and enter the city.

3. **Object upgrades & expansion**  
   Player spends accumulated resources to upgrade parking, cash desks, unlock new desks and purchase upgrades that increase income.

4. **City development**  
   Continuous improvement of infrastructure and efficiency leads to higher income and progression.

5. **Cycle repetition**  
   After upgrades and management actions the loop repeats at a higher level of efficiency.

---

### Testing Approach (based on STLC)

1. **Requirement Analysis**  
   Studied the provided GDD fragment (Parking, Cash Desks, Station, Cafe, Helicopter, Offline return, Core Loop).  
   Goal: understand game logic, identify ambiguities, define key objects for testing.

2. **Test Planning**  
   Defined scope, priority areas (economy, queues, NPC flow, rewarded mechanics) and testing types (functional, exploratory).

3. **Test Case Development**  
   - Created a structured checklist (20 items)  
   - Wrote 20 test cases covering core mechanics, UI, boundary and negative scenarios  
   - Linked test cases to potential defects

4. **Test Environment Setup**  
   Installed the provided APK on an Android device.

5. **Test Execution**  
   - Executed checklist and test cases  
   - Performed exploratory testing focused on UX and core loop  
   - Verified income generation, queues, upgrades and rewarded features

6. **Defect Reporting**  
   Documented 6 bugs with full structure (steps, expected vs actual result, priority).

7. **Test Cycle Closure**  
   Summarized results, core loop analysis and remaining ambiguities in the GDD.
