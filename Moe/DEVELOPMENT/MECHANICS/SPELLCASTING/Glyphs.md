**Glyphs** are the symbols that are needed in order to complete spells in combat, exploration, and puzzle solving.

*What kinds of glyphs are there?*
* Most glyphs are *active glyphs* - they are chosen and employed by the player at their discretion
* There are some *passive glyphs* - mostly contextual, signpost-style glyphs that are used for narrative purposes. An example is Moe's glyph which will indicate the presence of a saferoom.

*How does a player learn glyphs?*
* The player learns a glyph by first encountering it in the game. This is done by interacting with enemies, an item, or an environmental effect.
	* Example: The player encounters an enemy in the kitchen. They know that they want to try to release this enemy. Observing the enemy shows that the player needs to learn a glyph in order to release it. They hunt down an important item related to the monster. After psychometrically analyzing it, they learn the glyph and it is added to their glyph wheel for later use.

*What do glyphs actually do?*
* **Combat** - Glyphs are used to weaken enemies so they can be killed or released. 
* **Environmental Effects** - Some environmental effects are triggered by glyphs, such as pulling an item off a wall or remotely opening a door
* **Puzzle** - Some puzzles require a glyph to solve to remove a magical barrier blocking progression
* **Exploration** - A trail of glyphs can 

## **2. GLYPH SYSTEM**

### **Overview**

Glyphs are magical symbols that represent weaknesses in enemies and locks in the environment. Players must learn glyphs and use them to complete enemy "glyph sequences" (locking them in place) or solve environmental puzzles (opening doors, dispelling barriers).

---

### **Glyph Types**

#### **Narrative Glyphs (Permanent)**

**Purpose:** Story progression and exploration

**Properties:**

- Found through exploration and psychometry
- Added to permanent codex (never lost)
- Used for: Unlocking doors, dispelling barriers, ritual puzzles
- Always available once learned

**Examples:**

- Moe's Personal Glyph (tutorial, inherent)
- Named Character Glyphs (Sorceress, Warlock, key NPCs)
- Location-specific Glyphs (Farm Seal, Boundary Ward)

**Acquisition:**

- Story beats (given during key moments)
- Psychometry (touching significant objects reveals glyphs)
- Environmental clues (inscriptions, altars, ritual circles)

---

#### **Combat Glyphs (Temporary)**

**Purpose:** Enemy weaknesses and tactical tools

**Properties:**

- Learned by focusing on enemies during combat
- Added to temporary glyph pool (quick-slot menu)
- Can be cleared manually (make room for new glyphs)
- Lost on death? **No** - persist on retry (knowledge retained)

**Common Combat Glyphs:**

- Circle (basic, common enemy type)
- Triangle (basic, common enemy type)
- Square (intermediate)
- Pentagon (intermediate)
- Octagon (intermediate)
- Hexagon (advanced)
- Heptagon (advanced, rare)

---

### **Glyph Learning System**

#### **First Encounter (Unknown Glyph)**

**Process:**

1. Enemy appears with floating glyph icon (fuzzy/unclear)
2. Player focuses on enemy (hold focus button, no charging yet)
3. After 2 seconds: Glyph clarifies and is added to temporary pool
4. Visual feedback: Icon sharpens, success chime
5. Glyph now available in wheel menu

**Psychometry Acceleration (Optional):**

- While focusing, hold psychometry button
- Glove removal animation plays (0.5 seconds)
- Learning time reduced: 2 seconds → 1 second
- **Cost:** Mandragora meter increases +15%
- **Risk/Reward:** Faster learning vs. stalker danger

**Key Points:**

- Learning is vulnerable (can be interrupted by attacks)
- Focus breaks if player takes damage
- Learning progress does NOT drain (commitment-free)

---

#### **Subsequent Encounters (Known Glyph)**

**Process:**

1. Enemy appears with same glyph type
2. Glyph instantly clear and recognizable (no fuzzy period)
3. Automatically added to temporary pool if not already present
4. No focus needed - immediate identification
5. Can begin charging immediately

**Design Intent:**

- Rewards experience (you've fought this before)
- Faster subsequent encounters (no learning phase)
- Encourages observation and memory

---

### **Temporary Glyph Pool**

**Capacity:** 6 glyphs maximum

**Management:**

- **When full:** Player must choose which glyph to replace (manual selection)
- **Clear All:** Button to empty entire pool (useful after changing areas)
- **Prioritization:** Player decides which glyphs are most valuable

**UI Display:**

- Shows currently held glyphs (Circle, Triangle, Square - 3/6 slots used)
- Quick-access during combat (separate from weapon radial menu)
- Visual indicator when pool is full (cannot learn new glyphs)

**Strategic Considerations:**

- Keep common glyphs (Circle, Triangle) for frequent enemies
- Clear unused glyphs before new area
- Pool persists on death (no re-learning penalty)

---

### **Glyph Charging (Combat)**

#### **Manual Focus Charging**

**Process:**

1. Equip desired glyph from wheel menu (0.5-second animation)
2. Aim at enemy, hold focus button
3. Camera locks onto target
4. Progress bar fills over time (base: 4 seconds)
5. Taking damage breaks focus
6. If focus broken: Progress drains over 2 seconds
7. Complete glyph: Enemy locks in place (5-second stun)

**Visual Feedback:**

- Enemy has floating glyph icon showing current required glyph
- Progress bar fills around icon (circular meter)
- Enemy body glows when glyph is being charged
- Flash + distinct audio when glyph completes

**Interruption:**

- Any damage to player breaks focus
- Progress drains at 50% per second
- If re-focus before fully drained: Resume from current progress
- If fully drained: Start over from 0%

---

#### **Ritual Passive Charging**

**Process:**

1. Ritual placed with matching glyph slots (e.g., Athame has Circle + Triangle)
2. Enemy with matching glyph enters ritual zone
3. Glyph automatically charges at 25% per second (33% for Staff)
4. No player input required (fully passive)
5. Visual: Subtle pulsing around enemy

**Active + Passive Stacking:**

- If player focuses on enemy with matching ritual slot: Both effects stack
- Example: Athame Circle slot (25%) + Player focus (50%) = 75% per second
- Wand with focus boost: 25% passive + 75% active = 100% per second (instant)

---

#### **Glyph Sequences**

**Single-Step Sequences (Basic Enemies):**

- Require only 1 glyph to lock
- Example: Corrupted Thrall = Circle only
- Once complete: Enemy locked, can kill or release

**Multi-Step Sequences (Advanced Enemies):**

- Require 2-3 glyphs in specific order
- Example: Corrupted Warden = Circle → Triangle → Square
- Must complete glyphs sequentially (cannot skip)
- Each completion: Brief lock (2 seconds), then glyph switches to next in sequence
- Final glyph completion: Full lock (5 seconds)

**Glyph Display:**

- Current glyph shown as floating icon above enemy
- Completed glyphs: Dim/grey (already done)
- Active glyph: Bright/glowing (currently needed)
- Remaining glyphs: Faded (upcoming)

**Sequence Example (Warden):**

1. Enemy appears with Circle icon (bright)
2. Player completes Circle → Enemy locks briefly, icon changes to Triangle
3. Player completes Triangle → Enemy locks, icon changes to Square
4. Player completes Square → Enemy fully locked (can kill/release)

---

### **Glyph Resolution**

#### **Kill Option**

**Process:**

1. Enemy fully locked (all glyphs completed)
2. Attack enemy with any weapon
3. Enemy health depletes normally
4. Death: Enemy dissolves, leaves material component (crafting resource)

**Rewards:**

- Material components for crafting consumables
- Immediate threat removal
- No mana refund

---

#### **Release Option**

**Process:**

1. Enemy fully locked (all glyphs completed)
2. Press release button (1-second animation)
3. Enemy dissolves peacefully (no drops)
4. Full mana refund (100 mana restored)

**Rewards:**

- Complete mana restoration (powerful)
- Moral choice (mercy over violence)
- Possible narrative consequences (release "count" tracked?)

**Requirements:**

- Some enemies have special release conditions (must find object first)
- Use psychometry on locked enemy to learn condition
- Example: "This creature cherished a locket" → find locket → bring to enemy → release possible

---

### **Glyph Usage in Puzzles**

**Environmental Locks:**

- Doors, barriers, chests have glyph slots (usually 2-3 slots)
- Use Chalk consumable to reveal required glyphs
- Place ritual near object with matching glyphs
- When glyphs "charge" in ritual zone, lock opens

**Ritual Altars:**

- Special locations require specific glyph rituals
- May require narrative glyphs (story progression gates)
- Multiple altars may need simultaneous activation
- Teaches: Rituals have non-combat applications

**Example Puzzle:**

- Door has 3 slots: Circle, Triangle, Square
- Place Athame ritual (has Circle + Triangle slots)
- Circle and Triangle charge → 2/3 complete
- Must manually focus Square glyph OR place second ritual with Square
- When all 3 charged: Door unlocks
