**Mana** is the basic resource that the player will spend to complete in-game actions such as casting spells, making (and using) some items, defeating enemies, or solving puzzles.

*What uses Mana?*
- Spellcasting and magic attacks
- Rituals
- Quick item crafting
- Enhanced psychometry
- Remote item movement ("psychokinesis"/"telekinesis")

*What does not use Mana?
* Standard game actions like walking, collecting and using items, talking to living people, etc.
* Basic psychometry
* Release
* Puzzles (even magical ones)

*How do you restore Mana?*
* Wait - mana restores slowly over time (slower on hard mode?)
* Mana springs - naturally occurring pools of mana that will appear in areas of heavy magic use
* Releasing an enemy - restores a significant portion of the player's mana (all on lower difficulties, only some on higher?)
* Advanced glyphs that require timing, such as a perfectly countered spell or a well-executed glyph placement
* Save points - restore mana on use (instant/increased regen speed? -> facilitates note reviews)
* Learning a new glyph

*What happens when you're out of Mana?*
* No spellcasting
* Full exhaust = longer regent start time?
* Full exhaust = increased Mandragora spawn chance?

**Mana Banking**
Mana Banking (name tbd) is a technique players will be able to use to softly invest the amount of mana they've used in an action so they can divert their focus without having to worry about starting completely over.

*Example:* Moe finds herself facing two enemies. She spends some time working one subduing one, but finds that the one she hasn't been focusing on is much closer. She can *bank* the mana she used thus far so the glyph progress on one enemy doesn't fully decay on the other enemy so she can deal with the other enemy (fight, flee, or start subduing this one)

*Variable information:*
Type - Float
Max - 100.0
Min - 0.0
Current - XXX.XX
Upgradeable - No (unlikely)

## **3. MANA & RESOURCE MANAGEMENT**

### **Overview**

Mana is the primary resource for all magical actions (attacks, rituals, glyph charging). Players must balance spending mana on offense/defense while maintaining enough for critical actions. The mana lock system adds a layer where players can "freeze" progress at the cost of reducing their available mana pool.

---

### **Mana Pool**

**Base Stats:**

- **Maximum Mana:** 100 (baseline, may increase through upgrades)
- **Starting Mana:** 100 (full at encounter start)
- **Regeneration Rate:** 2 mana per second (passive, always active unless stated otherwise)

**Visual Display:**

- Blue bar below health bar
- Shows current/maximum (e.g., "75/100")
- Locked mana displayed as dimmed/darker section
- Low mana warning: Pulses when below 25%

**Audio Feedback:**

- Gentle hum when regenerating
- Low mana warning sound at 25%
- Depleted sound when hitting 0 mana
- Cannot cast when at insufficient mana (error sound)

---

### **Mana Costs**

#### **Weapon Attacks:**

|Weapon|Attack|Cost|
|---|---|---|
|Athame|Light Bolt|10|
|Wand|Heavy Bolt|25|
|Bell|AOE Shockwave|40|
|Staff|Melee Strike|15|
|Telekinetic Throw|Environmental Throw|10|

#### **Ritual Actions:**

|Action|Cost|
|---|---|
|Place Ritual|30 (one-time on deployment)|
|Dismiss Ritual|0 (free)|
|Glyph Charging (Focus)|0 (free while focusing, but blocks regen)|
|Mana Lock|Amount locked × 1 (e.g., 40% progress = 40 mana locked)|

**Note on Glyph Charging:**

- Focusing on enemy does NOT cost mana directly
- However, mana regeneration pauses while focusing (opportunity cost)
- Extended focus = missed regeneration = indirect cost

---

### **Mana Lock System**

#### **Purpose**

Allows players to "freeze" glyph progress on enemies to prevent decay when switching targets or being interrupted. Locked progress is preserved, but the mana spent is temporarily unavailable for other actions.

---

#### **Lock Mechanics**

**Activation:**

1. Glyph partially charged (any percentage: 10%, 50%, 90%)
2. Press Lock button (L1/LB or equivalent)
3. Mana equal to progress percentage is locked
4. Example: 60% progress on Circle glyph = 60 mana locked

**Visual Feedback:**

- Locked mana: Darker blue section on mana bar with chain icon
- Available mana: Bright blue (usable)
- Text display: "40/100 Mana Available" (60 locked)
- Locked glyph: Small lock icon appears next to enemy's glyph

**Locked Mana Behavior:**

- Locked mana CANNOT be spent on attacks, rituals, or other actions
- Maximum mana effectively reduced by locked amount
- Multiple glyphs can be locked simultaneously (additive cost)
- Example: Lock 30% on Enemy A, 40% on Enemy B = 70 mana locked, only 30 available

---

#### **Decay Prevention (Key Feature)**

**Without Lock:**

- Stop focusing on enemy → progress drains at 50% per second
- 2 seconds = total loss

**With Lock:**

- Stop focusing on enemy → progress FROZEN for 5 seconds (grace period)
- Grace timer counts down (5... 4... 3... 2... 1...)
- After 5 seconds: Decay begins normally (50% per second)
- Resume focusing before decay: Timer resets, progress preserved

**Strategic Use:**

- Lock Enemy A → focus Enemy B for 4 seconds → return to Enemy A (grace still active)
- Enables multi-enemy juggling without losing progress
- Grace timer pauses while actively focusing that enemy (only counts down when NOT focusing)

**Visual/Audio:**

- Grace timer: Countdown numbers appear on locked glyph (5... 4... 3...)
- Warning: Audio cue at 1 second remaining (urgent beep)
- Decay start: Visual pulse when grace expires

---

#### **Unlock Mechanics**

**Manual Unlock:**

1. Press Lock button again while targeting locked enemy
2. Instantly reclaims locked mana (returns to available pool)
3. **Prototype:** No penalty (full refund)
4. **Potential Full Game:** 5-10% penalty on unlock (lose some mana as "tax")
5. Progress preserved (can re-lock later)

**Automatic Unlock:**

- Complete glyph → automatic unlock of that glyph's mana
- Full refund (no penalty)
- Example: 60 mana locked on Circle, complete it → 60 mana returns

**Death/Reset:**

- All locks released on player death
- Mana resets to full (100) on retry
- Must re-learn/re-lock in next attempt

---

#### **Strategic Depth**

**Multi-Enemy Scenarios:**

- Enemy A at 50% (lock 50 mana) → Enemy B appears → focus Enemy B
- Return to Enemy A before 5-second grace expires
- Finish both without losing progress

**Risk/Reward:**

- Lock too much: Shrinking mana pool limits combat options (can't afford shockwave, rituals)
- Lock too little: Risk losing progress if interrupted
- Finding balance: Core skill expression

**Death Spiral Tension:**

- Lock 30% on Enemy A (30 mana)
- Lock 40% on Enemy B (40 mana)
- Only 30 mana available for attacks/defense
- High tension: Must complete locked glyphs to reclaim mana
- Failure to complete: Stuck in low-mana state

---

### **Mana Recovery Methods**

#### **Passive Regeneration**

- 2 mana per second (always active)
- Continues during combat, rituals, movement
- **Only interruption:** While actively focusing on enemy (pauses regen)

#### **Release Enemy**

- Full mana refund: 100 mana instantly
- Requires all glyphs completed first
- Mercy option: No materials but massive mana gain

#### **Salt Consumable (in Ritual)**

- Boosts regen to 22 mana per second (base 2 + 20 from Salt)
- Duration: 30 seconds
- Must be inside ritual zone to benefit

#### **Pop Projectiles (Defensive Ritual)**

- Complete glyph on enemy projectile in ritual zone
- Projectile dissolves, refunds 15 mana
- Sustainable defense: Pop attacks → regain mana → pop more attacks

#### **Consumable Items (Outside Ritual)**

- **Essence Vial:** +50 mana instantly (rare drop/find)
- **Mana Draught:** +100 mana (full refill, very rare)
- Limited quantity, must be crafted or found

---

### **Mana at Zero**

**Consequences:**

- Cannot cast any attacks (all weapons require mana)
- Cannot place rituals (30 mana cost)
- CAN still: Move, dodge, interact, dismiss rituals
- Essentially defenseless if cornered by enemies

**Recovery from Zero:**

- Passive regen: 2/sec = 50 seconds to full (very slow)
- Release enemy: Immediate 100 mana (if enemy locked)
- Use consumable: Instant refill (if available)
- Dismiss ritual and reposition: Stall until mana recovers

**Design Intent:**

- Running out of mana is serious but not instant death
- Encourages resource management (don't spam expensive attacks)
- Makes release option tempting (trade materials for mana)