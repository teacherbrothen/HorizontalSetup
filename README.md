# Horizontal Projectile Motion Setup

An interactive, web-based scaffolding tool designed for high school physics students learning 2D kinematics. 

This activity isolates **problem translation and conceptual modeling** from mathematical calculation. Before students begin crunching numbers or manipulating algebraic formulas, this tool trains them to parse word problems, organize independent dimensions into a T-Chart, assign correct coordinate vector signs, identify implicit projectile constants, and locate the critical bridge variable ($t$).

---

## 🎯 Pedagogical Rationale

Physics Education Research (PER) demonstrates that novice physics students often struggle with kinematics word problems not because they cannot perform arithmetic, but because of **excessive cognitive load**. Novices attempt to juggle reading comprehension, coordinate system conventions, formula recall, and calculator work simultaneously.

This tool isolates schema development through a deliberate 4-step framework:

1. **Decoupling Dimensions (The T-Chart):** Reinforces that horizontal motion (constant velocity) and vertical motion (constant acceleration due to gravity) are completely independent.
2. **Metacognitive Sign Reflection:** When a student places a given value into the chart, they are prompted to declare whether it is positive or negative. This forces them to treat values as vectors with direction rather than absolute numbers (e.g., recognizing that falling off a $25\text{ m}$ cliff corresponds to a vertical displacement of $\vec{d}_V = -25\text{ m}$).
3. **Activating Implicit Givens (Knowledge Bank):** Word problems rarely state that an object is launched horizontally with an initial vertical velocity of $0\text{ m/s}$ or that downward acceleration is $-9.81\text{ m/s}^2$. Students must identify these "hidden" constants from a bank that includes common conceptual distractors.
4. **Targeting the Bridge Variable ($t$):** Students learn to look for the column containing 3 known variables and recognize that scalar time ($t$) must be calculated first to cross over and solve for the unknown in the opposite column.

---

## ✨ Features

- **No Calculation Required:** Focuses entirely on setting up the problem.
- **Isotropically Scaled Motion Diagram:** Features an SVG diagram where vertical cliff height and horizontal range are rendered at an authentic 1:1 scale relative to the randomized values. The target unknown is displayed as a `?`.
- **Natural Language Parsing:** Avoids orphaned trailing punctuation and uses varied linguistic representations (chronological, outcome-first, question-first, passive/technical).
- **Randomized Problem Sequence:** Scenarios and numerical values are randomized for every student and session.
- **Chromebook & Windows Optimized:** Clean sans-serif math rendering via KaTeX with vector arrows anchored strictly over variable symbols.
- **LMS / Brightspace Integration:** Built-in SCORM 1.2 engine reports a 100% completion grade once 5 problems are solved, with grade-locking logic allowing unlimited subsequent practice.
- **Verification Clipboard Proof:** Includes an `html2canvas` button that captures a timestamped proof card with a unique session ID for students to paste directly into LMS discussions or dropboxes.

---

## 🚀 Quick Deployment Options

### Option A: Host on GitHub Pages (Standalone Web Activity)
1. Fork or push this repository to GitHub.
2. Go to **Settings** $\rightarrow$ **Pages**.
3. Under **Branch**, select `main` (or `master`) and folder `/root`, then click **Save**.
4. Share the generated URL with your students or embed it in your LMS via an `<iframe>`:
   ```html
   <iframe src="https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/" width="1000" height="900" frameborder="0"></iframe>
