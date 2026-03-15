#  BreakOrNot
> \*\*AI-powered sprain vs. fracture assessment in 60 seconds.\*\*  
> No hospital. No X-ray. No ₹5,000 bill.
![BreakOrNot Hero](https://img.shields.io/badge/status-prototype-yellow) ![License](https://img.shields.io/badge/license-MIT-green) ![Tech](https://img.shields.io/badge/stack-HTML%20%2F%20CSS%20%2F%20JS-blue) 
---
📌 The Problem
From Razorpay's Fix My Problem hackathon challenge:
> \*"Why is distinguishing sprains from fractures impossible without costly hospital visits?"\*
Millions of people in India visit emergency rooms every year for soft tissue injuries — waiting 3–5 hours and spending ₹3,000–₹8,000 — only to be told "rest it, it's probably fine." Most of these visits are avoidable with proper triage.
BreakOrNot solves this with a clinical symptom-scoring model that gives an instant, structured assessment — for free.
---
✨ Features
5-step symptom assessment — mechanism, location, pain level, weight-bearing, visible signs
Weighted clinical scoring — logic mirrors the Ottawa Ankle/Foot Rules used by triage nurses
3-tier result system — Likely Sprain / Possibly Fractured / Likely Fracture
Actionable next steps — tailored RICE instructions, when to visit a clinic, when to go to A&E
Photo upload — FileReader API preview (CV analysis in future version)
Free doctor consultation — connect with an orthopedic specialist via video call
Zero dependencies — pure HTML, CSS, JS. No frameworks, no installs
Fully responsive — works on any device

🛠️ Tech Stack
Layer	Technology
Frontend	Vanilla HTML5, CSS3, JavaScript (ES6+)
Typography	Syne (display) + DM Sans (body) via Google Fonts
Styling	CSS Custom Properties (design tokens), no preprocessor
Animations	CSS keyframes + `cubic-bezier` spring curves
Scroll effects	`IntersectionObserver` API
Image handling	`FileReader` API
Hosting	Static — deployable anywhere
Why no framework?
This is a hackathon prototype. Vanilla JS keeps it zero-dependency, instantly deployable as a single `.html` file, and fast to iterate. A production version would use React + a real ML backend.

🧠 Scoring Algorithm
The fracture probability score is calculated from weighted clinical indicators:
```
score = mechanism + pain\_bonus + weight\_bearing + swelling + bruising + deformity + numbness

fracture\_probability = min(95, max(8, score × 2.2))
```
Or deploy instantly:
https://breakornot.vercel.app/

📁 Project Structure
```
breakornot/
├── index.html          # Entire app — single file, self-contained
├── README.md           # You are here
```

⚠️ Disclaimer
BreakOrNot is a prototype and is not a medical device or substitute for professional medical care.
Do not rely on this tool for emergency decisions
In an emergency, call 112 or go to your nearest A&E
Always consult a qualified healthcare professional for injuries

📄 License
MIT — free to use, modify, and distribute.

<div align="center">
  Made with ❤️.
</div>
 
