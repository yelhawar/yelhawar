## Hi, I'm Yahia 👋

First-year **Honours Computer Science + Business Administration** (double degree) student at the **University of Waterloo** and Wilfrid Laurier University. I like problems that sit between math, software, and the physical world: scientific machine learning, rocket software, data-heavy interfaces, and tools people actually use.

- 🔭 Open to **Summer 2027 co-op / internship** roles in software, ML and data
- 📚 Currently taking MATH 145 (Algebra, Advanced), MATH 147 (Calculus, Advanced) and CS 145 (Designing Functional Programs, Advanced)
- 🌍 Languages: Arabic (native), English, French (fluent), German (proficient)
- 📫 [linkedin.com/in/yelhawary](https://www.linkedin.com/in/yelhawary) · yahia.hawary@gmail.com

---

### 🚀 Waterloo Rocketry · Software Engineer · *Oct 2026 – Present*
*Student design team building and launching rockets at the University of Waterloo.*

- Primarily responsible for the **SD-card subsystem**, working alongside the software lead: SD-card integration and on-board **data logging** for the rocket's software systems
- Collaborating on the team's new **[launch application](https://github.com/waterloo-rocketry/launch-app)** (React + TypeScript + Electron), which supports rocket launch operations
- Focus: embedded and software systems, data logging, launch software

### 🧪 [PINN vs. Classical ODE Fitting](https://github.com/yelhawar/PINN-Projectile-Motion-EE) · Python, PyTorch, SciPy · *Completed*
*Can a physics-informed neural network recover an unknown physical parameter from noisy data better than classical curve fitting?* (IB Physics Extended Essay)

- Built a PINN in PyTorch that recovered the **drag coefficient** of a projectile from **60 noisy observations** to within **0.25%** of ground truth, compared with **12.4%** error for SciPy least-squares ODE fitting
- Embedded the drag ODE directly in the loss function using **second-order autograd**, and made the drag coefficient a **trainable softplus parameter** so it always stays physically positive
- Trained in two stages (**Adam → L-BFGS**), cutting the loss by about six orders of magnitude, and explained why each optimizer was needed from the training curve
- Diagnosed *why* the classical baseline failed (errors in the estimated initial velocity leaking into the drag estimate), and documented the study's limitations honestly, including the lack of a held-out test split
- The repo is reproducible: fixed seeds, one script, and the results table and figures regenerate exactly

### 🖥️ Waterloo Terminal · *Co-creator* · React, TypeScript, Vite · *In development*
*A "Bloomberg Terminal" for student opportunities: clubs, events, research, jobs and the people connected to them, modelled as a graph so students can see what to do next and recruiters can see who is high-signal.*

I co-created the project and designed and built its **"motherboard" interface**. Specifically, I:
- **Wrote the visual-analytics engine** (`insights.ts`, ~700 lines), which computes every analysis view live from the session's node graph:
  - **Pipeline:** a Sankey diagram of where people come from before an opportunity and where they go after it
  - **Path:** the most probable **Markov-chain walk** from the user to a target opportunity, shown as a subway line with per-hop transition probabilities
  - **Gap:** compares the user with people who landed an opportunity (topic and prior-step coverage, plus missing steps to collect)
  - **Signal:** **PageRank** rankings of people and organizations across six time cutoffs, drawn as a bump chart (who is rising)
  - **Horizon, Activity, Landscape and "since you last looked":** a deadline radar, a weekly club-activity heat grid, a radial topic map, and rank movers between visits
- **Designed and built the "motherboard" workspace,** the app's main tiled interface, including insight tiles, **workspace tabs** (each tab is its own tile mosaic), and click / double-click behaviour on every item
- **Designed and built a Student / Enterprise switch**, which adds an enterprise view with Talent radar, Outreach, Talent sources and Event ROI panels (opt-ins and replies are simulated for now)
- **Assembled the design lab:** static HTML explorations, wireframes and a component gallery behind the locked designs
- The repo is private while we build. Code is available on request.

### 🧭 Waterloo Platoon · Recruiting & Team Workspace · TypeScript, React, Cloudflare · *In development, not yet deployed*
*One workspace for a student team: applicants apply, admins run the recruiting pipeline, and members coordinate. I'm building it solo.*

- **Applicant portal:** open roles, applications with PDF/DOCX résumé upload (up to 10 MB), progress tracking and interview responses
- **Admin pipeline:** applicant filtering, board and list views, private notes, ratings, application stages and interview scheduling
- **Team workspace:** channels with threads, mentions and reactions, plus restricted and admin-only channels, meetings with RSVPs and calendar (.ics) downloads, and tasks, goals and deadlines
- **Contribution score:** a transparent formula (delivery, efficiency, effectiveness, commitment over 90 days) written as pure, unit-tested functions so members can see exactly how they're measured
- **Security:** Google OAuth with PKCE, single-use login state, hashed server-side sessions and same-origin logout. Permissions for organizations and channels are enforced in the API handlers, and new accounts never become admins automatically
- **Stack:** React + TypeScript on Cloudflare Workers, D1 (SQLite) with Drizzle ORM migrations, R2 file storage, Vitest tests and GitHub Actions CI
- Runs locally today; deployment is next

---

### 📐 Research & investigations
- **Stochastic modelling of Luxembourg rainfall** (IB Mathematics AA IA, completed). Analyzed **31 rainfall events**, modelled interarrival times with an **exponential distribution** and estimated its parameter, then used the model to estimate rainfall probabilities and system-capacity thresholds.
- **Bifilar pendulum & oscillatory motion** (IB Physics IA, completed). Designed and ran an experiment on how suspension geometry affects the oscillation frequency of a suspended metal rod: repeated timing measurements, uncertainty analysis and comparison with theory.
- **Cancer biology & UV radiation labs** (Scienteens Academy, University of Luxembourg). Supervised lab work on skin-cancer cell cultures, UV effects on bacterial DNA, and spectrometric analysis of sunscreen protection.

### 🏆 Competitions
- **AI Cafe Lux Competition: 3rd place, €1,000 (2024).** Designed a framework that turns engineering requirements into machine-checkable constraints, to flag unsafe construction calculations instead of trusting unconstrained generative-AI output. I was the youngest presenter and the only high-school competitor among 7 finalists.
- **Economics World Cup: Finalist (2025).** Analyzed Brazil's graphite industry and the EV supply chain, and presented policy recommendations with a team.
- **Harvard Crimson Global Case Competition (2025).** Built a strategic recommendation as part of a three-person team.
- **VEX Robotics: Lead Engineer (2022–2023).** Led the mechanical and electrical design; diagnosed drivetrain chain slippage and rewired the motors for torque and reliability.

### 🤝 Leadership
- **STEM Revision Club: Founder (2025–2026).** Founded a peer-led STEM revision club at the International School of Luxembourg and grew it from 1 to 20 students within its first month. I led the revision sessions in math and science.

### 🛠️ Tools I use
**Languages:** Python · TypeScript · SQL · Racket · Lean · LaTeX
**ML / scientific:** PyTorch · SciPy · NumPy · pandas · scikit-learn · matplotlib
**Web:** React · Vite · Cloudflare Workers / D1 / R2 · Drizzle ORM · Google OAuth · Vitest · GitHub Actions
