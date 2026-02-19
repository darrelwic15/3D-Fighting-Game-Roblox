# 3D-Fighting-Game-Roblox

 A prototype 3D fighting game framework built on Roblox. This project was developed as a hands-on exploration into advanced combat scripting, custom animation, and dynamic visual effects. It features a fully functioning real-time PvP combat system complete with advanced hit detection, state management, and custom VFX.


# Core Features
 Real-Time PvP: Fully replicated and optimized for fast-paced, real-time player-versus-player combat.

 Comprehensive Combo System: Supports fluid ground and aerial combat. Players can string together light/heavy attacks and launch opponents into the air for devastating air combos.

 Advanced Player Status System: A robust state machine that accurately tracks and detects player states in real-time to determine interaction logic. Tracked states include:
 - Stunned
 - In-Combo (Hitstun/Combo lock)
 - In-Air (Airborne status for aerial mechanics)
 - Block & Block-Broken

 Flashstep (Shunpo): High-speed movement mechanic inspired by Bleach. Includes custom particle trails and effects to emphasize speed and distance covered.

 Energy Attacks: Custom-scripted projectile and beam attacks created by repurposing and manipulating visual effect assets into fully playable, hitbox-active energy strikes.

# ---------------------------------------------------------------------------------------------------------------------------------------

# Animations and Visual effects
 A major focus of this project was learning and implementing high-quality visuals and animations alongside the code:

 Moon Animator Integration: All combat animations (idle stances, punches, kicks, hit reactions, and air juggles) were hand-crafted from scratch using the Moon Animation Editor plugin to ensure smooth, impactful movement.

 Roblox Particle System: Heavy utilization of Roblox's built-in ParticleEmitter class to create impactful visual feedback for hits, dashes, and energy charges.

 Dynamic Crater Generation: Engineered a system that generates physical/visual craters on the environment during heavy slams or specific high-impact attacks, greatly enhancing the game's "game feel" and combat weight.


# ---------------------------------------------------------------------------------------------------------------------------------------

# Technical Details
 Developer Note: This project served as a massive learning milestone. Bridging the gap between raw scripting (handling hitboxes, server-client replication, and state management) and visual artistry (animating in Moon Animator and tuning particle emitters) was the primary goal.

 Hit Detection: Optimized to ensure fairness in real-time PvP environments, compensating for latency where possible.

 State Machine: The combat flow relies on strict status checks (e.g., an attack will only land if the target is not currently in an invulnerable/dodging state, or a blockbreak is triggered if hit while blocking).
