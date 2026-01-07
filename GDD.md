# Iron Heresy - Game Design Document

## 1. Game Overview

### 1.1 Game Concept
**Title:** Iron Heresy  
**Genre:** Action Side-Scroller, Pixel Art  
**Platform:** PC (Windows)  
**Target Audience:** Fans of action platformers, retro gaming enthusiasts  

**Elevator Pitch:**  
[A brief 2-3 sentence description of your game - to be filled in]

### 1.2 Story & Setting

#### World
[Describe the game world, setting, and atmosphere]

#### Story Synopsis
[Main narrative arc - what's the player's journey?]

#### Main Characters
- **Protagonist:**
  - Name:
  - Background:
  - Motivation:
  - Abilities:

- **Antagonist(s):**
  - Name:
  - Background:
  - Role in story:

#### Key Story Beats
1. [Opening/Tutorial]
2. [Act 1]
3. [Act 2]
4. [Climax]
5. [Resolution]

---

## 2. Gameplay Mechanics

### 2.1 Core Gameplay Loop
[Describe what the player does moment-to-moment]

### 2.2 Player Controls

#### Movement
- **Walk/Run:** Left/Right arrow keys or A/D
- **Jump:** Spacebar or W (Height based on hold duration)
- **Double Jump:** Press jump again in air
- **Crouch:** Down arrow or S
- **Dash/Dodge:** [Define key]

#### Combat
- **Light Attack:** [Define key] - Fast, low damage
- **Heavy Attack:** [Define key] - Slow, high damage
- **Special Ability 1:** [Define key and ability]
- **Special Ability 2:** [Define key and ability]
- **Block/Parry:** [Define key]

#### Other Actions
- **Interact:** E key
- **Inventory:** I key
- **Pause Menu:** ESC

### 2.3 Combat System

#### Combo System
- [Define combo chains]
- Example: Light → Light → Heavy = "3-hit combo"

#### Damage Types
- Physical
- [Elemental if applicable]
- [Special damage types]

#### Hit Feedback
- Screen shake intensity
- Hit pause duration (frame freeze)
- Particle effects
- Sound effects

### 2.4 Player Progression

#### Leveling System
- Experience gained from: [enemies, collectibles, etc.]
- Level up rewards: [health increase, new abilities, stat boosts]

#### Skill Tree / Upgrades
[Define upgrade paths]
- Branch 1: [Combat focused]
- Branch 2: [Mobility focused]
- Branch 3: [Defense/Utility focused]

#### Equipment System
- Weapons: [List types]
- Armor: [List types]
- Accessories: [List types]

---

## 3. Enemy Design

### 3.1 Enemy Types

#### Basic Enemies
1. **[Enemy Type 1]**
   - Health: [amount]
   - Damage: [amount]
   - Behavior: [patrol, chase, attack pattern]
   - Drops: [items/XP]

2. **[Enemy Type 2]**
   - Health:
   - Damage:
   - Behavior:
   - Drops:

3. **[Enemy Type 3]**
   - Health:
   - Damage:
   - Behavior:
   - Drops:

#### Elite/Mini-Boss Enemies
1. **[Elite Enemy 1]**
   - Health:
   - Special abilities:
   - Attack patterns:
   - Drops:

#### Boss Enemies
1. **[Boss 1 Name]**
   - Location: [Level/Area]
   - Health:
   - Phase 1 attacks:
   - Phase 2 attacks:
   - Weakness:
   - Reward:

### 3.2 AI Behaviors
- **Patrol:** Random movement within area
- **Chase:** Pursue player when in detection range
- **Attack:** [Define attack patterns]
- **Retreat:** [When low health, if applicable]

---

## 4. Level Design

### 4.1 Level Structure
**Total Levels:** [Number]  
**Average Completion Time:** [Minutes per level]

### 4.2 Level Breakdown

#### Level 1: [Name] - Tutorial
- **Theme:** 
- **Length:** [Short/Medium/Long]
- **Objectives:**
  - Learn basic movement
  - Learn combat
  - Defeat first enemy
- **Enemies:** [Types and quantities]
- **Boss:** None
- **Collectibles:** [Number and types]

#### Level 2: [Name]
- **Theme:**
- **Length:**
- **Objectives:**
- **Enemies:**
- **Boss:**
- **Collectibles:**

[Continue for all levels...]

### 4.3 Checkpoint System
- Checkpoints placed every [X] screens
- Auto-save on checkpoint
- Respawn at last checkpoint on death

### 4.4 Secrets & Collectibles
- **Hidden Areas:** [Number per level]
- **Collectible Types:**
  - Health upgrades
  - Ability scrolls
  - Lore items
  - Currency/resources

---

## 5. Art & Audio

### 5.1 Visual Style

#### Pixel Art Specifications
- **Base Resolution:** 320x180 (scaled up 4x to 1280x720)
- **Sprite Size:** 32x32 pixels for characters
- **Tile Size:** 16x16 pixels
- **Animation Framerate:** 8-12 FPS

#### Color Palette
[Define your color palette - consider using tools like Lospec]
- Primary colors: [List hex codes]
- Secondary colors:
- Accent colors:
- UI colors:

#### Visual Effects
- Attack trails: [Color/style]
- Hit effects: [Particles, flashes]
- Environmental effects: [Fog, rain, etc.]

### 5.2 Animation List

#### Player Character
- Idle (4-6 frames)
- Walk (6-8 frames)
- Run (6-8 frames)
- Jump (3-4 frames)
- Fall (2-3 frames)
- Attack 1 (4-6 frames)
- Attack 2 (4-6 frames)
- Hurt (2-3 frames)
- Death (6-8 frames)

#### Enemies
[List animations per enemy type]

### 5.3 Audio Design

#### Music Tracks
1. Main Menu Theme - [Mood/style]
2. Level 1-3 Theme - [Mood/style]
3. Level 4-6 Theme - [Mood/style]
4. Boss Battle Theme - [Mood/style]
5. Victory Theme - [Mood/style]

#### Sound Effects Categories
- **Player Actions:** Jump, land, attack, hurt, death
- **Enemy Sounds:** Aggro, attack, hurt, death per enemy type
- **Environmental:** Footsteps, ambience, interactive objects
- **UI:** Button click, menu navigation, pause, collect item
- **Combat:** Hit impact, block, parry, special abilities

---

## 6. User Interface

### 6.1 HUD Elements
- **Health Bar:** Top left, red bar with heart icon
- **Energy/Stamina Bar:** Below health, blue/yellow bar
- **Experience Bar:** Bottom of screen, thin bar
- **Currency Counter:** Top right
- **Ability Icons:** Bottom right, show cooldowns

### 6.2 Menu Screens

#### Main Menu
- New Game
- Continue
- Settings
- Credits
- Exit

#### Pause Menu
- Resume
- Settings
- Controls
- Return to Main Menu

#### Settings Menu
- Graphics (Resolution, Fullscreen, VSync)
- Audio (Master, Music, SFX volumes)
- Controls (Key rebinding)
- Accessibility (Colorblind mode, screen shake toggle)

---

## 7. Technical Specifications

### 7.1 Engine & Technology
- **Engine:** Godot 4.x
- **Programming Language:** GDScript
- **Resolution:** 1280x720 (16:9 aspect ratio)
- **Target Framerate:** 60 FPS

### 7.2 System Requirements

#### Minimum
- **OS:** Windows 10 (64-bit)
- **Processor:** Intel Core i3 or equivalent
- **Memory:** 4 GB RAM
- **Graphics:** Integrated graphics
- **Storage:** 500 MB available space

#### Recommended
- **OS:** Windows 10/11 (64-bit)
- **Processor:** Intel Core i5 or equivalent
- **Memory:** 8 GB RAM
- **Graphics:** Dedicated GPU with 2GB VRAM
- **Storage:** 1 GB available space

### 7.3 Controls Support
- Keyboard & Mouse (primary)
- Xbox Controller (optional)
- PlayStation Controller (optional)

---

## 8. Development Milestones

### 8.1 Prototype Phase (Month 1-2)
- [ ] Basic player movement
- [ ] Simple combat system
- [ ] 1 test level
- [ ] 1 enemy type

### 8.2 Alpha Phase (Month 3-4)
- [ ] All core mechanics implemented
- [ ] 3-5 levels complete
- [ ] 3-5 enemy types
- [ ] Basic UI

### 8.3 Beta Phase (Month 5-6)
- [ ] All levels complete
- [ ] All enemies and bosses
- [ ] Full UI/UX
- [ ] Playtesting and balancing

### 8.4 Polish Phase (Month 7-8)
- [ ] Bug fixing
- [ ] Performance optimization
- [ ] Final art and audio
- [ ] Marketing materials

---

## 9. Monetization & Distribution

### 9.1 Pricing Strategy
- **Free:** [If free-to-play]
- **Paid:** $[X.XX] USD
- **Early Access:** [If applicable]

### 9.2 Distribution Platforms
- [x] Steam
- [ ] itch.io
- [ ] Epic Games Store
- [ ] GOG

### 9.3 Marketing Plan
- Social media presence (Twitter, Reddit, Discord)
- Dev blog/YouTube devlog
- Press kit and game trailer
- Demo release
- Influencer outreach

---

## 10. Post-Launch Plans

### 10.1 Updates & Patches
- Bug fixes
- Performance improvements
- Quality of life improvements

### 10.2 DLC/Expansion Ideas
[List potential additional content]

---

## Appendix

### A. References & Inspiration
[List games, art, music that inspire your game]
- Gameplay: [Game 1], [Game 2]
- Art Style: [Game 1], [Game 2]
- Music: [Artist], [Soundtrack]

### B. Resources
- [Link to asset folders]
- [Link to development tools]
- [Link to documentation]

---

**Document Version:** 1.0  
**Last Updated:** [Date]  
**Author:** [Your Name]
