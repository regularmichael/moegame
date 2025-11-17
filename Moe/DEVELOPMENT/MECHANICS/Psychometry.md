#### **Overview**

Moe's curse/gift allows her to see the history of objects by touching them bare-handed (removing magical gloves). This ability is essential for investigation but attracts the Mandragora (stalker entity) when used excessively.

---

#### **Basic Psychometry Use**

**Activation:**

1. Approach object with psychometry option (prompt appears)
2. Hold interact button
3. Gloves auto-remove (animation, 0.5 seconds)
4. Vision/flashback plays (length varies: 2-15 seconds)
5. Release button to end early OR vision completes
6. Gloves auto-return

**Vision Types:**

- **Light Read (2-5 sec):** Environmental clues, object history (low detail)
- **Medium Read (5-10 sec):** Character memories, moderate emotional content
- **Deep Read (10-15 sec):** Traumatic events, critical story revelations (intense)

**Information Revealed:**

- Object origin/purpose
- Last person to touch it
- Emotional imprints (fear, joy, anger)
- Hidden clues (combination numbers, secret paths)
- Glyph knowledge (narrative glyphs learned through visions)

---

#### **Mandragora Threat Meter (Hidden)**

**Meter Properties:**

- 0-100% scale (not visible to player)
- Increases with psychometry use
- Decays slowly over time (2-3% per minute when not using psychometry)
- Story moments can force meter to 100% (scripted Mandragora encounters)

**Meter Increases:**

- Light read: +5-10%
- Medium read: +15-25%
- Deep read: +30-50%
- Combat psychometry (learning glyphs faster): +20-30%

**Feedback to Player (No UI):**

**25-50% (Early Warning):**

- Audio: Distant whispers, faint breathing
- Visual: Shadows slightly longer
- Moe's audio: Slightly labored breathing after psychometry

**50-75% (Clear Danger):**

- Audio: Whispers resolve into fragmented words ("...found you...")
- Visual: Lights flicker, peripheral shimmer
- Environmental: Flowers wilt momentarily

**75-100% (Imminent Spawn):**

- Audio: Clear footsteps, Moe gasps "It's close..."
- Visual: Screen vignette darkens, brief Mandragora silhouettes
- Music: Drops to single sustained drone

**100%+ (Spawn Guaranteed):**

- Next psychometry use triggers Mandragora spawn
- Or spawns at next story-appropriate moment

---

#### **Combat Psychometry Applications**

**Glyph Learning Acceleration:**

- While focusing on enemy to learn glyph (normal: 2 seconds)
- Hold psychometry button during focus
- Learning time: 2 seconds → 1 second
- Meter increase: +20-30%
- Risk/reward: Faster knowledge vs. stalker danger

**Release Condition Discovery:**

- Touch locked enemy (all glyphs completed)
- Vision shows: "This creature cherished a locket..."
- Reveals location of object needed for release
- Enables mercy option (peaceful resolution + full mana)
- Meter increase: +25-35%

---

### **Mandragora (Stalker Entity)**

#### **Overview**

A supernatural pursuer attracted by excessive psychometry use. Cannot be killed, only evaded or temporarily escaped. Becomes more dangerous as game progresses.

---

#### **Spawn Behavior**

**Spawn Conditions:**

- Meter reaches 100% (guaranteed spawn on next psychometry use)
- Or meter 75%+ and story trigger point
- Or scripted story moment (overrides meter)

**Spawn Location:**

- Out of player's view (behind, around corner, distant room)
- On or near path to nearest safe room (blocks direct route)
- Always positioned to create tension (not impossible to avoid, but challenging)

---

#### **Mandragora States**

**State 1: Hunting (Initial)**

- Moves toward player's last known psychometry location
- Speed: Slightly slower than player sprint
- Detection: Line-of-sight based, wide FOV (120°)
- Behavior: Methodical room searching, checks hiding spots randomly
- Audio: Footsteps, dragging sounds, inhuman breathing

**State 2: Tracking (Active Psychometry)**

- If player uses psychometry while Mandragora active
- Speed: Matches player sprint
- Knows exact player location (beelines directly)
- No longer searches, just pursues
- Audio: Faster footsteps, breathing intensifies

**State 3: Escalation (Late-Game Abilities)**

**Teleportation (Mid-Game):**

- After losing line of sight for 30+ seconds
- Teleports closer to player (15-20m away)
- Audio: Sudden silence → loud manifestation sound
- Prevents camping in one hiding spot

**Stunning Scream (Late-Game):**

- When player in line of sight at medium range (10-15m)
- 3-second windup (Mandragora inhales, screen distorts)
- Effect: Stuns player for 2-3 seconds, drains 20 mana
- Counterplay: Break line of sight during windup OR get very close/far

**Free-Roaming Body Parts (End-Game):**

- Mandragora splits off tendrils/root clusters
- 1-2 additional entities patrol separately (smaller, weaker)
- Main body still pursues player
- Forces player into more dangerous positions (can't just flee down one path)

---

#### **Mana Drain Aura**

**Proximity-Based Tiers:**

- **Far (30+ meters):** No drain, but audio cues present (you know it's near)
- **Medium (15-30 meters):** -1 mana per second
- **Close (5-15 meters):** -3 mana per second
- **Very Close (<5 meters):** -5 mana per second
- **Line of Sight:** +2 additional mana per second (regardless of distance)

**Example:**

- Mandragora 10m away, no line of sight: -3 mana/sec
- Mandragora 10m away, line of sight: -5 mana/sec
- Mandragora 3m away, line of sight: -7 mana/sec

**Strategic Implications:**

- Can't just hide and wait (mana drains, eventually helpless)
- Breaking line of sight reduces drain (incentive to hide, then move)
- Must escape or reach safe room before mana depletes
- At 0 mana: Can't fight normal enemies, completely vulnerable

---

#### **Escape Options**

**Distance:**

- Maintain 40+ meters for 60+ seconds
- Mandragora gives up, dissolves
- Difficult: Requires knowing level layout, planning route

**Hiding:**

- Enter closet, under furniture, crawlspace
- Mandragora searches area for 15-20 seconds
- Must stay still/quiet (button hold to stay quiet?)
- If player moves or makes noise: Detected
- Success: Mandragora moves to different area, can sneak away

**Safe Room:**

- Enter safe room (designated room with clear visual marker)
- Instant Mandragora dismissal
- Meter drops to 50% (not zero - still elevated risk)
- Safe rooms are sparse (1-2 per major area)

**Environmental:**

- Close/lock doors behind you (delays Mandragora, doesn't stop)
- Collapse hallways with environmental triggers (psychometry reveals these)
- Knock over objects to create noise distractions elsewhere

---

#### **De-Spawn**

**Conditions:**

- Time: 2-3 minutes of activity without catching player
- Distance: Player maintains distance threshold for 60+ seconds
- Safe room: Instant
- Story trigger: Certain moments force dismissal

**Visual:**

- Mandragora dissolves into roots/vines
- Sinks into ground/walls
- Audio: Retreating sounds, whispers fade
- Relief moment: Music returns to normal, tension release