# Checklist

Structured checklist for a mobile idle / city-builder game (details anonymized).

### 1. Launch & Basic Stability
| # | Check | Expected Result | Priority | Status |
|---|-------|-----------------|----------|--------|
| 1 | Game launches without errors | Game starts successfully, main menu is displayed | High | Passed |

### 2. Parking & Vehicles
| # | Check | Expected Result | Priority | Status |
|---|-------|-----------------|----------|--------|
| 2 | Cars automatically enter parking | Cars enter free parking slots when available | High | Passed |
| 3 | Parking queue fills correctly | When all slots are occupied, cars wait in the queue | Medium | Passed |
| 4 | Income is generated from occupied slots | Income increases according to the number of parked cars | High | Passed |
| 5 | Parking level upgrade | Number of slots and income per slot increase after upgrade | High | Passed |
| 6 | Purchase of income upgrades | Income per slot increases according to the upgrade effect | Medium | Passed |

### 3. Cash Desks & NPC Flow
| # | Check | Expected Result | Priority | Status |
|---|-------|-----------------|----------|--------|
| 7 | NPCs move to cash desks | NPCs go to the nearest available cash desk | High | Passed |
| 8 | Cash desk processes NPC | Cash desk accepts payment, NPC proceeds further | High | Passed |
| 9 | Overloaded cash desk behavior | Desk is marked as overloaded, new NPCs go to departure | Medium | Passed |
| 10 | Cash desk level upgrade | Desk parameters update and level increases | High | Passed |
| 11 | Building a new cash desk | New cash desk appears after purchase | High | Passed |
| 12 | NPCs progress in the queue | NPCs move forward in queue slots after previous ones are processed | High | Passed |

### 4. NPC Generation & Timing
| # | Check | Expected Result | Priority | Status |
|---|-------|-----------------|----------|--------|
| 13 | NPC generation by train | Train arrives and brings NPCs at the defined interval | Medium | Passed |

### 5. Buildings & Passive Income
| # | Check | Expected Result | Priority | Status |
|---|-------|-----------------|----------|--------|
| 14 | Autonomous building work | Building generates income even without NPCs | Low | Passed |
| 15 | Cafe passive income | Cafe automatically generates currency | Medium | Passed |
| 16 | Unlocking Cafe #3 | Cafe #3 becomes available after building the 2nd building | Medium | Passed |

### 6. Offline, Rewarded & Special Mechanics
| # | Check | Expected Result | Priority | Status |
|---|-------|-----------------|----------|--------|
| 17 | Return after offline | Offline reward is shown with an option to increase it | Medium | Passed |
| 18 | Watch video to double income | After watching the ad, income is multiplied by 2 | High | Passed |
| 19 | Use hard currency for higher multiplier | Income is multiplied by the stated factor after spending hard currency | Medium | Passed |
| 20 | Helicopter appears periodically | Helicopter arrives and offers to watch an ad | Low | Passed |
