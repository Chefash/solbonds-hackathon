# ☀️ SOLBonds - Sustainable NFT Matchmaking Protocol

> NFT dating game meets DeFi yield - where compatibility earns real rewards

## 🎯 The Problem
Traditional NFT projects promise unsustainable APRs that inevitably drain reward pools and collapse, leaving users with worthless tokens and broken promises.

## 💡 Our Solution
SOLBonds is a matchmaking protocol where NFT pairs earn sustainable rewards based on:
- **Compatibility Score** (0-100%): Better matches = higher multipliers
- **Bond Duration**: Longer commitment = exponential rewards
- **Real DeFi Yield**: Backed by Solana's best protocols, not printed tokens

## 🔥 Key Features

### Compatibility Algorithm
Multi-factor matching system:
- **Gender Alignment** (20%): Masculine/Feminine preference matching
- **Zodiac Compatibility** (30%): Astrological harmony (Fire, Earth, Air, Water)
- **Pet Preferences** (25%): Dog person + Cat person = conflict!
- **Risk Tolerance** (25%): Trading behavior compatibility

Result: 0-100% compatibility score that determines reward multipliers.

### Time-Based Reward Tiers
| Duration | Daily Rate | Multiplier | Example Earnings |
|----------|-----------|------------|------------------|
| Days 1-7 | 0.5% | 1.0x | $0.28/day |
| Days 8-30 | 1.0% | 1.5x | $0.84/day |
| Days 31-90 | 2.0% | 2.5x | $2.80/day |
| Days 91-180 | 3.5% | 4.0x | $7.84/day |
| Days 181+ | 5.0% | 6.0x | $16.80/day |

*Based on 50K vault, 50 active pairs, 85% compatibility*

### Compatibility Multipliers
- 90-100% compatibility: **2.0x** 🔥 (Soulmates)
- 80-89% compatibility: **1.5x** 💕 (Great match)
- 70-79% compatibility: **1.2x** 💛 (Good match)
- 60-69% compatibility: **1.0x** ⚡ (Base rate)
- Below 60%: **0.8x** 😅 (Penalty - risky match!)

## 💰 Sustainable Economics

### Revenue Sources (Daily)
```
Total Daily Inflow: $55.96

├─ DeFi Vault Yield: $10.96/day (8% APY on $50K)
│  ├─ 40% Kamino Finance ($20K @ 24% APY)
│  ├─ 25% MarginFi ($12.5K @ 12% APY)
│  ├─ 15% Sanctum ($7.5K @ 6% APY)
│  ├─ 10% Orca Treasury ($5K @ 5% APY)
│  └─ 10% SolBlaze LST ($5K @ 7% APY)
│
├─ User Activity Fees: $45/day
│  ├─ Mint Fees ($5 × 5 users/day)
│  ├─ Breakup Penalties ($5 × 2 breakups/day)
│  ├─ Discovery Bets ($1-10, avg $5 × 2/day)
│  └─ Boost Stakes ($3 × 3 users/day)
```

### The Formula
```javascript
Daily Earnings = (Real Yield + User Fees) ÷ Active Pairs × Time Tier × Compatibility

Example:
($55.96 ÷ 50 pairs) × 2.0 (Tier 3) × 1.5 (85% compat) = $3.36/day per pair
```

### Why It's Sustainable
✅ **No Printed Tokens**: Only distribute real revenue
✅ **Growing Vault**: Principal compounds via DeFi yield
✅ **Multiple Revenue Streams**: Not reliant on new users
✅ **Deflationary Pressure**: Breakup fees replenish pool
✅ **Transparency**: All numbers visible on dashboard

## 🎮 User Experience Flow

1. **Profile Creation** ($5 mint fee)
   - Choose gender preference
   - Select zodiac sign
   - Pick pet preference
   - Set risk tolerance

2. **Discovery Phase** (Optional boosts)
   - $1: Get 1 personality hint
   - $3: See top 3 potential matches
   - $5: Full compatibility report
   - $10: Priority matching queue

3. **Matching**
   - Algorithm calculates compatibility
   - 48-hour acceptance window
   - Both parties must accept

4. **Bonding**
   - NFTs visually "merge"
   - Earnings start immediately
   - Dashboard shows real-time rewards
   - Claimable USDC accumulates daily

5. **Relationship Management**
   - Stay bonded: Earnings compound
   - Break up early: Pay $5 penalty
   - Break up after 90 days: $2 fee
   - Break up after 180 days: Free

## 🛠️ Technical Implementation

### Tech Stack
- **Frontend**: HTML5, Tailwind CSS, Vanilla JavaScript
- **Blockchain**: Solana (SPL Tokens, Metaplex NFTs)
- **Smart Contracts**: Anchor Framework (planned)
- **DeFi Integration**: Kamino, MarginFi, Sanctum, Orca, SolBlaze
- **Automation**: Clockwork (daily reward distribution)

### Smart Contract Architecture (Planned)
```rust
// Core Programs
1. NFT Minting Program (Metaplex)
2. Profile Management Program
3. Matching Engine Program
4. Bond Management Program
5. Reward Distribution Program
6. Vault Management Program
```

### Key Data Structures
```rust
pub struct UserProfile {
    pub owner: Pubkey,
    pub nft_mint: Pubkey,
    pub gender_pref: u8,
    pub zodiac_sign: u8,
    pub pet_preference: u8,
    pub risk_level: u8,
    pub compatibility_hash: [u8; 32],
}

pub struct BondAccount {
    pub nft_a: Pubkey,
    pub nft_b: Pubkey,
    pub bond_start: i64,
    pub compatibility_score: u8,
    pub last_claim: i64,
    pub total_earned: u64,
    pub tier: u8,
}
```

## 📊 Example Economics (90-Day Projection)

**Launch Conditions:**
- 100 NFTs minted: $500 → Vault
- Initial vault: $50,000 USDC
- 50 pairs formed

**Day 30:**
- Vault grown to $50,328 (compound yield)
- 40 pairs still bonded (10 broke up → $50 penalty fees)
- Average daily earnings: $1.20/pair

**Day 60:**
- Vault: $50,656
- 45 pairs bonded (5 new matches)
- Average daily earnings: $1.48/pair

**Day 90:**
- Vault: $50,985
- 50 pairs bonded
- Top earners (Tier 4, 95% compat): $8.40/day
- Lowest earners (Tier 1, 65% compat): $0.32/day

**ROI Example:**
- User paid $5 mint fee
- Found 92% compatibility match
- Stayed bonded 90 days
- Total earnings: $168
- ROI: 3,260% 🚀

## 🏆 Why SOLBonds Wins

### Innovation
✅ First protocol combining NFT matchmaking + sustainable DeFi yield
✅ Compatibility-weighted rewards (unique mechanism)
✅ Social treasury management wrapper

### Product Quality
✅ Beautiful, intuitive UI with smooth animations
✅ Complete user flow (onboarding → earning → claiming)
✅ Real-time reward calculations
✅ Transparent economics dashboard

### Technical Execution
✅ Multi-protocol DeFi integration strategy
✅ Sustainable tokenomics (no infinite minting)
✅ Privacy-preserving compatibility algorithm
✅ Automated daily reward distribution

### Market Fit
✅ Solves NFT utility problem
✅ Gamifies DeFi yield in accessible way
✅ Viral potential ("My NFT is in a relationship")
✅ Real financial incentives for engagement

## 🚀 Roadmap

### Phase 1: MVP (Hackathon)
- ✅ Compatibility algorithm
- ✅ Time-based reward tiers
- ✅ Sustainable tokenomics model
- ✅ Frontend demo
- ⏳ Smart contract deployment

### Phase 2: Launch
- Deploy to Solana mainnet
- Integrate Kamino Finance
- Real USDC vault
- NFT art generation
- Mobile app

### Phase 3: Scale
- AI-powered compatibility (ChatGPT)
- "Double Date" mode (4-way bonds)
- NFT trait evolution
- Cross-chain expansion
- Dating app partnerships

### Phase 4: Ecosystem
- $BOND governance token
- Community treasury
- Partner integrations
- IRL meetup events

## 📹 Demo & Links

- **Live Demo**: 
- **Video Walkthrough**: 
- **GitHub**: https://github.com/Chefash/SOLBonds
- **Twitter**: [@solbondsNFT](https://x.com/solbondsNFT)
- **Email**: [SolBonds.NFT@yahoo.com](https://solbonds.NFT@yahoo.com)
- **Discord**:https://discord.gg/zF2edcJNCJ 

## 👥 Team

Built by a passionate vibes coder for the Indie.fun Hackathon 2025.

## 📄 License

MIT License - Build on it, fork it, make it yours!

---

**Built for Indie.fun Hackathon 2025** | Solana DeFi × Social Gaming | ☀️ Find Your SOLmate
