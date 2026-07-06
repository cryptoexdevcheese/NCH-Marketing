# NCH-Marketing: Standalone Binary MLM Engine & Web Dashboard

A high-performance, standalone **Binary Multi-Level Marketing (MLM) Engine** and **Interactive Tree Dashboard** for NCH (Native Cheese Coin).

---

## 🌟 Key Features

1. **Dual-Leg Binary Tree Engine**: Supports Left Leg (`L`) and Right Leg (`R`) placement.
2. **Extreme Spillover Logic**: Automatic downline placement when a sponsor's immediate branch is occupied.
3. **Weaker-Leg 10% Binary Matching Bonus**: Calculates 10% on the weaker leg volume and automatically carries over the remaining volume on the strong leg.
4. **Daily Safety Caps & Anti-Gaming**: Enforces daily payout caps per wallet (default: 1,000 NCH/day) to safeguard token supply and prevent inflation.
5. **Interactive Tree Visualizer**: Visual rendering of downline generations, leg volumes, and carryovers.
6. **Zero Dependencies on `cheese-blockchain` core repo**: Completely isolated, standalone repository.

---

## 📁 Repository Structure

```
nch-marketing/
├── package.json               # Project manifest
├── server.js                  # Express API Server
├── mlm-engine.js              # Core Binary MLM Engine
├── db.js                      # SQLite Database Layer
├── render.yaml                # Render Blueprint Configuration
├── public/                    # Frontend Dashboard UI
│   ├── index.html             # Glassmorphism Dashboard
│   ├── styles.css             # Styling & Animations
│   └── app.js                 # Web3 Wallet Connect & Tree Rendering
└── test/                      # Verification Test Suite
    ├── test-mlm.js            # Core Engine Tests
    └── test-server-endpoints.js# Express HTTP Endpoint Tests
```

---

## 🚀 Local Setup & Testing

### 1. Install Dependencies
```bash
npm install
```

### 2. Run Test Suite
```bash
npm test
```

### 3. Start Local Server
```bash
npm start
```
Visit: `http://localhost:4000`

---

## 🌐 Deployment to GitHub & Render (`johnrobsteser3@gmail.com`)

### Step 1: Link Remote Repository
```bash
git remote add origin https://github.com/johnrobsteser3/NCH-Marketing.git
git branch -M main
git push -u origin main
```

### Step 2: Render.com Blueprint Setup
1. Log in to Render.com under `johnrobsteser3@gmail.com`.
2. Click **New +** -> **Blueprint**.
3. Select GitHub repository: `NCH-Marketing`.
4. Render automatically detects `render.yaml` and deploys the Node web service.
