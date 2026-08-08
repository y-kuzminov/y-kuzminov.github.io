# Test Cases

Test cases for a mobile idle / city-builder game (details anonymized).

---

### TC_01 — Car enters parking slot
**Priority:** High  
**Status:** Passed  
**Preconditions:** Free parking slot is available  

**Steps:**
1. Launch the game
2. Wait for a car to appear
3. Observe the car behavior

**Expected Result:**  
Car enters a free parking slot. Slot becomes occupied.

---

### TC_02 — Parking queue fills correctly
**Priority:** Medium  
**Status:** Passed  
**Preconditions:** Parking has a limited number of slots (e.g. 3)

**Steps:**
1. Wait until more cars arrive than available slots
2. Observe parking and queue

**Expected Result:**  
Available slots are filled first. Extra cars wait in the queue.

---

### TC_03 — Income generation from parking
**Priority:** High  
**Status:** Passed  
**Preconditions:** At least one parking slot is occupied

**Steps:**
1. Wait several seconds
2. Check currency balance

**Expected Result:
- Currency balance increases over time
- Income amount corresponds to the number of occupied parking slots

---

### TC_04 — Parking level upgrade
**Priority:** High  
**Status:** Passed  
**Preconditions:** Player has enough currency

**Steps:**
1. Open parking upgrade
2. Tap the upgrade button
3. Observe changes

**Expected Result:**  
Parking level increases. Number of slots and/or income per slot increases.

---

### TC_05 — Purchase income upgrade
**Priority:** Medium  
**Status:** Passed  
**Preconditions:** Income upgrade is available and player has enough currency

**Steps:**
1. Open upgrades menu
2. Purchase an income upgrade
3. Check income from parking slots

**Expected Result:**  
Income per slot increases according to the upgrade effect.

---

### TC_06 — NPC goes to cash desk
**Priority:** High  
**Status:** Passed  
**Preconditions:** At least one cash desk is free

**Steps:**
1. Wait for an NPC to appear
2. Observe NPC movement

**Expected Result:**  
NPC moves to the nearest available cash desk.

---

### TC_07 — Cash desk processes NPC
**Priority:** High  
**Status:** Passed  
**Preconditions:** NPC is in the cash desk queue

**Steps:**
1. Wait for the cash desk to process the NPC
2. Observe the result

**Expected Result:**  
Cash desk accepts payment. NPC proceeds further into the city.

---

### TC_08 — Overloaded cash desk behavior
**Priority:** Medium  
**Status:** Passed  
**Preconditions:** Cash desk queue is full

**Steps:**
1. Create a situation where the desk becomes overloaded
2. Observe new NPCs behavior

**Expected Result:**  
New NPCs are redirected to departure instead of joining the full queue.

---

### TC_09 — Cash desk upgrade
**Priority:** High  
**Status:** Passed  
**Preconditions:** Player has enough currency

**Steps:**
1. Tap the “Upgrade” button on a cash desk
2. Observe desk parameters

**Expected Result:**  
Cash desk level increases and its parameters are updated.

---

### TC_10 — Build a new cash desk
**Priority:** High  
**Status:** Passed  
**Preconditions:** Player has enough currency

**Steps:**
1. Tap “Build cash desk”
2. Confirm the action

**Expected Result:**  
A new cash desk appears in the game.

---

### TC_11 — NPC generation by train
**Priority:** Medium  
**Status:** Passed  
**Preconditions:** Game is running

**Steps:**
1. Note the time of the last train arrival (or start of the session)
2. Wait for the next train
3. Observe NPCs and income

Expected Result:
- Train arrives after the defined interval
- NPCs appear from the train
- NPCs can generate income after reaching cash desks

---

### TC_12 — NPCs progress in the queue
**Priority:** High  
**Status:** Passed  
**Preconditions:** Several NPCs are standing in the cash desk queue

**Steps:**
1. Wait for the first NPC to be processed
2. Observe the remaining NPCs

**Expected Result:**  
NPCs move forward in the queue slots after the previous one is processed.

---

### TC_13 — Autonomous building work
**Priority:** Low  
**Status:** Passed  
**Preconditions:** Building is already constructed

**Steps:**
1. Do not interact with the building
2. Wait and check income

**Expected Result:**  
Building generates income even without NPCs.

---

### TC_14 — Offline reward offer
**Priority:** Medium  
**Status:** Passed  
**Preconditions:** Player was offline for several minutes

**Steps:**
1. Return to the game
2. Observe the reward popup

**Expected Result:**  
Offline reward is shown with an option to increase it.

---

### TC_15 — Helicopter reward content
**Priority:** Medium  
**Status:** Failed  
**Preconditions:** Helicopter event is active

**Steps:**
1. Wait for the helicopter to appear
2. Tap on the reward offer
3. Check available rewards

**Expected Result:**  
Reward offer contains both Soft and Hard currency.

**Actual Result:**  
Only Soft currency is shown.

---

### TC_16 — Cash desk upgrade does not deduct money (according to GDD)
**Priority:** High  
**Status:** Failed  
**Preconditions:** Player has enough currency

**Steps:**
1. Note current balance
2. Tap “Upgrade” on a cash desk
3. Check balance again

**Expected Result (according to GDD):**  
Cash desk level increases and currency is **not** deducted.

**Actual Result:**  
Currency is deducted from the player balance.

---

### TC_17 — Train arrival interval
**Priority:** Medium  
**Status:** Failed  
**Preconditions:** Game is running

**Steps:**
1. Record time of one train arrival
2. Record time of the next train arrival
3. Calculate the difference

**Expected Result (according to GDD):**  
Train arrives every 60 seconds.

**Actual Result:**  
Train arrives approximately every 45 seconds.

---

### TC_18 — Maximum number of cash desks
**Priority:** High  
**Status:** Failed  
**Preconditions:** Player can build cash desks

**Steps:**
1. Build cash desks until the limit is reached
2. Count the total number of desks

**Expected Result (according to GDD):**  
Maximum 9 cash desks are available.

**Actual Result:**  
Only 8 cash desks can be built.

---

### TC_19 — Income multiplier for hard currency
**Priority:** High  
**Status:** Failed  
**Preconditions:** Player has enough hard currency

**Steps:**
1. Open the income multiplier offer
2. Purchase the multiplier
3. Check the applied multiplier and cost

**Expected Result (according to GDD):**  
Income is multiplied by 5 for 30 hard currency.

**Actual Result:**  
Income is multiplied by 3 for 20 hard currency.

---

### TC_20 — Capacity and queue data consistency
**Priority:** Medium  
**Status:** Failed  
**Preconditions:** Game is running, statistics screen is available

**Steps:**
1. Open statistics for buildings
2. Compare displayed capacity/queue values with actual behavior in the game

**Expected Result:**  
Statistics values match the actual capacity and queue size.

**Actual Result:**  
Displayed values do not match the real capacity and queue.
