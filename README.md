# QA Analysis: Gaia GPS, 
**Date:** 02/03/2026

**Reporter:** Quiana Caldwell

**Device:** iPhone 16 / iOS 26.2.1

**App Version:** v.2026.1

---
## 📋 Executive Summary
This repository contains a targeted Quality Assurance analysis of the Gaia GPS mobile application. The goal was to execute an ad-hoc test. Below I will report my findings

--- 
## 🛑 Critical Functional Bug
### [CRITICAL] 'Guide Me' CTA Fails to Load Trail Overlay (Null Map State)

* **Severity:** High / Blocker
* **Repro:** 100% 4/4 attempts
* **Summary:** When a user attempts to start their hike session via the 'Guide Me' button for desired trail, the application fails to pass the trail data to the Map View, resulting in an empty map without the selected trail navigation.
* **Steps to Reproduce:**
    1. Launch Gaia GPS and tap the **Magnifying Glass** icon to open the **'Discover'** modal.
    2. Select any specific trail (e.g., "Fagan Spring Loop via Railroad Bed Trail").
    3. Tap the Meatball menu icon to open secondary list of CTA's
    4. Tap the **'Guide Me'** CTA.
* **Actual Result:** Discover Modal is dismissed , The map resets to a default/generic view of the geographic area without trail indication.
* **Expected Result:** The map should initiate the navigation sequence with the selected trail highlighted and the user's GPS position centered.
* **Note:** I have performed this test as a core/free user 

**Video Evidence:** [🎥 Click here to view the Bug Report on Loom](https://www.loom.com/share/8550d5dbbac84b628351a216edef8563) 
