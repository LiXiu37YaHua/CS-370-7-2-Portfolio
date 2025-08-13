# CS-370-7-2-Portfolio
**Course:** CS-370-14243-M01 — Current/Emerging Trends in CS 202  
**Student:** Marissa Lanza

A simple, responsive personal web page for the **7-2 Portfolio Prep (Non-graded)** task.  
It showcases selected projects (e.g., Treasure Maze DQN, CartPole DQN, data dashboards), core skills, a short bio, and contact info.

## Live Site (optional)
If you publish with GitHub Pages, add the link here:
- **Live Demo:** https://YOUR-USERNAME.github.io/CS-370-7-2-Portfolio/

---

## Contents
├─ index.html # Single-page portfolio (Projects, Skills, About, Contact)
├─ styles.css # Accessible, responsive styling (light/dark ready)
├─ script.js # Theme toggle + current year
└─ README.md # This file
## Quick Start
**View locally**
1. Download/clone the repository.
2. Open `index.html` in your browser.

**Publish with GitHub Pages (recommended)**
1. Push to a public GitHub repo.
2. Go to **Settings → Pages**.
3. Set **Source** to `main` branch, `/ (root)` directory.
4. Save. Your site will be available at `https://YOUR-USERNAME.github.io/CS-370-7-2-Portfolio/`.

## Customize
Open `index.html` and update:
- **Projects**: Replace placeholder links with your repos/notebooks.
- **Skills**: Edit the pill list to match your stack.
- **About**: Short bio (keep it 3–5 lines).
- **Contact**: Email, GitHub, LinkedIn.

> Tip: Add alt text for any screenshots, e.g. `alt="Treasure Maze DQN path visualization"`.

## Tech Stack
- **HTML/CSS/JS** (no build tools required)
- Accessible, responsive layout (works on mobile & desktop)
- Light/Dark theme toggle

---

## Example Project Cards
Update the links to your work:
- **Treasure Maze DQN Agent** — Deep Q-learning agent that reaches the treasure using replay memory and ε-greedy exploration. *(Python, Keras/TensorFlow)*
- **CartPole DQN** — Balanced the pole via DQN; tuned ε schedule and buffer size for stability. *(Python, TensorFlow)*
- **Sales Dashboard (Power BI)** — Modeled SQL Server data; cut reporting time by ~40%. *(SQL Server, Power BI)*
- **Inventory Management (MySQL)** — Optimized queries and built CRUD endpoints. *(MySQL, REST)*

---

## Brightspace Submission Notes
For **7-2 Portfolio Prep (Web Page)**, submit:
- The **ZIP** of this site (`Lanza_Marissa_7-2_Portfolio.zip`)
- **One screenshot** of the homepage showing your name + sections
- (If allowed) the **live URL** to your GitHub Pages site

**Suggested submission comment:**  
> Single-page portfolio (Projects, Skills, About, Contact). Links point to my CS-370 work. Built with HTML/CSS/JS; accessible and responsive. No changes to Project Two `.py` files.
>
> ## CS 370 – Module Eight Journal (Portfolio Entry)

**Artifact:**  
- 📄 [TreasureHuntGame.ipynb](./TreasureHuntGame.ipynb)  <!-- TODO: update path if different -->
- (Optional) 🖼️<img width="1751" height="827" alt="image" src="https://github.com/user-attachments/assets/7788156d-d9c6-416b-927c-5923e9f2e2fd" />

- Add a screenshot of the agent’s final path: `images/maze-run.png`

### What I built (given vs. created)
- **Given:** Environment and replay classes; starter notebook cells; the maze and reward rules; a working model builder.
- **Created by me:** The **Q-Training Algorithm** (Deep Q-Learning loop) with ε-greedy action selection, experience replay training, valid-action masking, hyperparameters (γ, ε schedule, batch size), and early stopping once the rolling win rate hit 100%. I also added in-line comments and ran the “play/draw” demo to verify the learned path.

### Connecting learning to computer science
**What do computer scientists do and why does it matter?**  
We turn real-world problems into computable tasks, choose the right models and data structures, and build reliable systems that other people can use. That matters because small design choices (like reward shaping or data validation) directly impact safety, fairness, and user trust.

**How do I approach a problem as a computer scientist?**  
I define the objective and constraints, map them to the right abstractions (state, actions, rewards), and iterate: prototype → test → measure → refine. For this project, that meant starting with a clear reward function, using DQN for policy learning, and tuning ε/γ until the agent stopped wandering and converged.

**What are my ethical responsibilities to the end user and the organization?**  
Be transparent about system limits, avoid harmful side effects, and protect data. In RL terms, reward design should reflect true goals (no shortcuts or perverse incentives). In code, follow secure and maintainable practices so others can safely extend the work.

### Notes on the technique (brief)
- **Why DQN?** Scales better than a big Q-table, generalizes across states, and works well on small discrete mazes.  
- **Results:** Consistent wins; 100% rolling win rate → early stop (stable policy).  
- **Trade-offs:** Sample-inefficient vs. newer variants; sensitive to reward shaping; acceptable within course constraints.

**References (APA):** Lin (1992); Mnih et al. (2015); Sutton & Barto (2018).
