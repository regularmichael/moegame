Rituals are ways for players to use the environment to aid them in combat, exploration, and investigation. 
#### **Chalice**

**Role:** Ritual catalyst (required for all ritual placement)

**Weapon Properties:**

- No direct attack
- Always equipped/available
- Cannot be lost or dropped

**Ritual Properties:**

- Acts as anchor point for all rituals
- Must be placed before any ritual can be deployed
- Can accept consumables for enhanced effects
- Setup time: 0.5 seconds (placement) + 1.5 seconds (lighting)

**States:**

- **Unplaced:** In inventory, ready to deploy
- **Placed (Unlit):** On ground, can be picked up and repositioned without penalty
- **Lit (Active):** Committed to location, cannot be moved, waiting for item selection or timer active if consumable added
- **Deployed:** Full ritual active with chosen item

**Usage Notes:**

- Flexible setup order: Can light first (reactive play) or choose item first (planned play)
- Consumable timer starts when lit (creates urgency if lit before item chosen)
- Cannot have multiple Chalices placed simultaneously

### **Ritual System Mechanics**

#### **Ritual Placement Process**

**Step-by-Step:**

1. **Equip Chalice** from inventory
2. **Aim reticle** at ground location
3. **Place Chalice** (0.5-second animation)
	* **Add Consumable** (optional, instant from menu)
4. **Choose Item or Light** (player decides order):
    - Option A: Select ritual item → Light Chalice → Item deploys
    - Option B: Light Chalice → Wait for right moment → Select item → Item deploys
5. **Ritual Active** - Zone appears, item removed from weapon inventory

**Reposition Rules:**

- **If unlit:** Pick up Chalice instantly (no penalty, returns to inventory with consumable)
- **If lit:** Cannot pick up (committed to location)
- **If deployed:** Must dismiss entire ritual to move

**Dismissal:**

- Press dismiss button (instant)
- Ritual vanishes, item returns to weapon inventory
- Can immediately place new ritual elsewhere

---

#### **Ritual Zone Effects**

**Passive Glyph Charging:**

- Enemies with matching glyphs inside zone have their glyphs charge automatically
- Does NOT require player input (happens passively)
- Charge rate: 25% per second (33% for Staff)
- Visual: Gentle pulsing glow when enemy with matching glyph enters

**Active Focus Boost:**

- Player inside ritual zone focusing on enemy = accelerated charging
- Stacks with passive charging if glyph matches ritual slots
- Boost: 50% faster (75% for Wand)
- Visual: Brighter glow, more intense particle effects

**Stacking Example (Athame with Circle slot):**

- Enemy with Circle glyph enters zone: 25% passive charging per second
- Player focuses on same enemy from inside zone: 25% passive + 50% boost = 75% total per second
- Completes in ~1.3 seconds instead of 4 seconds

**Special Effects:**

- Bell: 30% movement slow to all enemies in zone
- Staff: Larger zone radius (10m vs 8m)
- Other items: No special effects beyond glyph charging + focus boost

---

#### **Ritual Limitations**

**One Ritual at a Time:**

- Cannot have multiple rituals active simultaneously
- Placing new ritual while one exists: Must dismiss first
- Design reason: Prevents overpowered "fortress" strategies, maintains tension

**Ritual Persistence:**

- Rituals remain active until manually dismissed
- Do not disappear on their own
- Persist through player movement (can leave zone and return)
- Destroyed if player dies (must replace on retry)

**Item Lock:**

- Item used in ritual is temporarily removed from weapon inventory
- Cannot use that weapon's attack while ritual is active
- Must dismiss ritual to regain weapon functionality
- Creates core tension: "Do I keep this as a weapon or place it as a ritual?"