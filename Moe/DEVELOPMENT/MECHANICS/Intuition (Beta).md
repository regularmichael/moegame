#### **Overview**

QTE-lite mechanic providing audiovisual cues for unseen dangers. Rewards player attention and provides accessibility without trivializing challenge.

---

#### **Trigger Contexts**

**Dodge Unseen Attacks:**

- Enemy about to attack from behind/off-camera
- Audio cue: Distinct "warning" sound (subtle whoosh)
- Visual cue: Silver line fills at screen edge (direction indicator)
- At apex: Press dodge button
- Success: Perfect dodge, brief invulnerability
- Failure: Take hit normally

**Stave Off Mandragora:**

- While using psychometry, Mandragora approaches
- Intuition prompt appears (same audio/visual)
- Press button to "stay alert"
- Success: Extends safe psychometry time by 3 seconds
- Failure: Mandragora meter increases faster

**Find Missable Clues:**

- Walking past hidden object/path
- Audio cue: Soft chime
- Visual cue: Subtle glow in direction of secret
- Follow prompt: Discover hidden item/area

---

#### **Design Principles**

**Never Mandatory:**

- Game completable without ever using intuition
- Missing prompts makes game harder, not impossible
- Optional assist system, not core mechanic

**Clear but Subtle:**

- Audio: Distinct, recognizable sound (not generic danger music)
- Visual: Screen-edge effect (not intrusive center prompt)
- Timing: Forgiving window (0.5-1 second, not frame-perfect)

**Consistent Language:**

- Same audio/visual for all intuition types
- Players learn "that sound means react now"
- No different cues per context (reduces learning curve)

**Toggleable:**

- Settings: Intuition Prompts (On / Off / Minimal)
- "Minimal" = audio only, no visual
- Accommodates player preference (hardcore vs. accessibility)

---

