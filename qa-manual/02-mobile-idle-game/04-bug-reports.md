# Bug Reports

Bug reports found during manual testing of a mobile idle / city-builder game (details anonymized).

---

### BUG_01 — Helicopter reward shows only one currency type
**Severity:** Medium  
**Priority:** Medium  
**Environment:** Android device  
**Preconditions:** Helicopter event is active  
**Related Test Case:** TC_15  
**Reproducibility:** High (reproduced consistently)

**Steps to Reproduce:**
1. Wait for the helicopter to appear in the game
2. Tap on the reward offer
3. Observe the available rewards

**Expected Result:**  
Reward offer contains both Soft and Hard currency.

**Actual Result:**  
Only Soft currency is shown (reproduced multiple times).

---

### BUG_02 — Cash desk upgrade deducts currency (contrary to GDD)
**Severity:** High  
**Priority:** High  
**Environment:** Android device  
**Preconditions:** Player has enough currency to upgrade a cash desk  
**Related Test Case:** TC_16  
**Reproducibility:** High

**Steps to Reproduce:**
1. Note the current currency balance
2. Tap the “Upgrade” button on a cash desk
3. Check the currency balance again

**Expected Result (according to GDD):**  
Cash desk level increases and currency is **not** deducted from the player balance.

**Actual Result:**  
Currency is deducted from the player balance after the upgrade.

---

### BUG_03 — Train arrival interval is shorter than specified
**Severity:** Medium  
**Priority:** Medium  
**Environment:** Android device  
**Preconditions:** Game is running  
**Related Test Case:** TC_17  
**Reproducibility:** High

**Steps to Reproduce:**
1. Record the time of one train arrival
2. Record the time of the next train arrival
3. Calculate the time difference

**Expected Result (according to GDD):**  
Train arrives every 60 seconds.

**Actual Result:**  
Train arrives approximately every 45 seconds.

---

### BUG_04 — Maximum number of cash desks is lower than specified
**Severity:** Medium  
**Priority:** Medium  
**Environment:** Android device  
**Preconditions:** Player can build cash desks  
**Related Test Case:** TC_18  
**Reproducibility:** High

**Steps to Reproduce:**
1. Build cash desks until the limit is reached
2. Count the total number of available cash desks

**Expected Result (according to GDD):**  
Maximum of 9 cash desks can be built.

**Actual Result:**  
Only 8 cash desks can be built.

> Note: Priority adjusted from High to Medium based on impact (game remains playable).

---

### BUG_05 — Income multiplier values do not match GDD
**Severity:** Medium  
**Priority:** Medium  
**Environment:** Android device  
**Preconditions:** Player has enough hard currency  
**Related Test Case:** TC_19  
**Reproducibility:** High

**Steps to Reproduce:**
1. Open the income multiplier offer
2. Check the multiplier value and cost
3. Purchase the multiplier and verify the applied effect

**Expected Result (according to GDD):**  
Income is multiplied by 5× for 30 hard currency.

**Actual Result:**  
Income is multiplied by 3× for 20 hard currency.

> Note: Priority adjusted from High to Medium (economy balancing issue, not a blocker).

---

### BUG_06 — Statistics show incorrect capacity and queue values
**Severity:** Medium  
**Priority:** Medium  
**Environment:** Android device  
**Preconditions:** Game is running and statistics screen is available  
**Related Test Case:** TC_20  
**Reproducibility:** High

**Steps to Reproduce:**
1. Open the statistics screen for buildings
2. Note the displayed capacity and queue values
3. Compare them with the actual number of visitors and queue size in the game

**Expected Result:**  
Statistics values match the actual capacity and queue size in the game.

**Actual Result:**  
Displayed values do not match real capacity and queue size  
(example: one building shows 36 in statistics but actually has 24 total places).
