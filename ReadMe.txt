OrchardApp 1.0.0
================

A SwiftUI + SpriteKit “Orchard of Ideas” prototype game. Tap to plant evolving hypothesis-trees, nurture them with simulated “watering” (evidence gathering), and build up your orchard of insight—while wilted saplings fade away. 

Overview
--------
In “Orchard of Ideas” you:

  • Plant a new hypothesis-seed (Linear, Quadratic, Cubic, Exponential, Sine, Log, Neural) by tapping the screen.  
  • Each tree grows one “age” per frame, accumulating “evidence” at a randomized rate.  
  • Trees whose evidence falls behind their age decay and turn gray—only healthy trees count toward your score.  
  • Your score is the sum of all alive trees’ evidence values.  
  • Strategize which seed to plant next to maximize your orchard’s resilience.

Key Files
---------
• OrchidApp.swift     — App entry point (SwiftUI @main).  
• ContentView.swift   — Hosts the SpriteKit OrchardScene in SwiftUI.  
• OrchardScene.swift  — SpriteKit scene implementing game logic and rendering.  
• README.txt         — This guide.

Requirements
------------
• Xcode 14 or later  
• iOS 15.0+ (or iPadOS 15.0+)  
• Swift 5.7+  
• SpriteKit & SwiftUI frameworks (built in)

Installation
------------
1. Clone or download this repository.  
2. Open `OrchardApp.xcodeproj` in Xcode.  
3. Select a Simulator (e.g. iPhone 14).  
4. Hit ⌘R to build & run.

Controls
--------
• **Tap anywhere** on the screen to plant a new tree at that location.  
• **Watch** each tree’s color, size, and evidence value to see how it fares.  
• **Score** and “Next seed type” are displayed at top of screen.

Customization
-------------
• Add or rename hypotheses by editing the `hypotheses` array in `OrchardScene.swift`.  
• Tweak growth dynamics in `TreeNode.water()`—adjust the evidence formula, decay threshold, or random factor.  
• Change visuals (colors, fonts, lighting) by modifying SKShapeNode and SKLabelNode properties.

Extending the Prototype
-----------------------
• Hook in real Monte Carlo evidence calculations (replace the random “water” step).  
• Add seasonal events—storms of doubt, rains of data, sunlight bursts—to affect all trees.  
• Introduce “weeds” or “pests” that attack weaker trees, requiring rapid replanting.  
• Persist high‐score orchards to disk or a cloud leaderboard.

License
-------
MIT License — see `LICENSE.txt` for full terms.

Author
------
Your Name – your.email@example.com

Enjoy cultivating your Orchard of Ideas!  
