# Creative Newtech: Scenario Valuation (Base / Bull / Bear vs CMP)
*As of 30-Sep-2026. All figures consolidated, ₹ crore unless per-share.*

## Step 1: Anchor facts

| Item | Value | Source |
|---|---|---|
| CMP | **₹1,104** | Bajaj Finserv markets page, close 29-Sep-2026 (other sites: ₹1,097–1,098 on 25–29 Sep) |
| Shares | 1.5017 cr basic; **1.5217 cr** including the proposed 2 lakh ESOPs | AR26 note 13; AGM notice |
| Mcap | ≈ ₹1,658 cr | CMP × 1.5017 cr |
| Owners' PAT | FY26 ₹61.9 cr (total ₹70.3 cr incl. NCI ₹8.4 cr) | AR26 consolidated P&L |
| EPS | FY26 ₹41.04; **TTM ₹43.35** (41.04 − 5.92 + 8.23) | AR26; Q1 FY27 deck |
| EBITDA | FY26 ₹104.0 cr; TTM ₹113.8 cr | May-26 call; Q1 FY27 deck |
| Net debt | ≈ **₹302 cr** (borrowings 324.3 − cash 5.4 − bank balances 16.8) | AR26 |
| Book value | Owners' equity ₹363.6 cr → BVPS ₹242.1 | AR26 |
| Current multiples | **P/E 25.5× TTM; P/B 4.6×; EV/EBITDA ≈ 17.4×** (EV ≈ ₹1,984 cr incl. NCI at book) | Computed |
| Own recent P/E | ≈16× (₹670, 14-May-26, on ₹41 EPS) and ≈21× (₹874, 13-Jul-26, TTM P/E 20.7 per share.market). The stock has re-rated from ~16× to ~25× in four months | Web, dated |
| Operating cash flow | FY26 −₹271.9 cr; free cash flow ≈ −₹275 cr | AR26 |

**Sector map:** trading/distribution (P/E, with EV/EBITDA as cross-check), plus a branded-consumer piece (P/E). Because the parts differ, a SOTP is shown in Step 6.

**Peer multiples:** not verified in this run. The multiple levels below are anchored on the stock's own 2026 range, and this is flagged as a limitation.

## Step 2: Assumption ledger (horizon FY27)

| Driver | Current | Base | Source / quote | Bull / Bear |
|---|---|---|---|---|
| Revenue growth | +52% FY26; +21% Q1 FY27 | **+20%** → ₹3,246 cr | Guidance "*at least in a year by 25%, 30%*" (May-26, p.8). Credibility LOW–MED: revenue promises are kept, so the discount is only small | Bull +30% (guidance) → ₹3,516 cr / Bear +5% (Middle East stress plus credit tightening) → ₹2,840 cr |
| PAT margin (incl. NCI) | 2.60% FY26; 2.84% Q1 FY27 | **2.4%** | Finance cost up 2.5× YoY in Q1 (₹7.63 cr vs ₹3.01 cr); brand EBITDA guided down to 13% (p.14) | Bull 2.8% / Bear 1.9% |
| NCI share of PAT | 12.0% FY26 | 12% | 22.5% of SCL | same |
| Shares | 1.5017 cr | 1.5217 cr (with ESOPs) | AGM notice | same |
| Margin guidance (4.5–5% PAT) | — | **ignored** | LOW credibility on margin/cash items (1 of 5 hit) | Not even used in Bull |

## Step 3: Section A — fundamental build

| Scenario | FY27 revenue | PAT margin | PAT (owners) | EPS | Exit P/E | Target | Gap to CMP |
|---|---|---|---|---|---|---|---|
| Bear | 2,840 | 1.9% | 47.5 | ₹31.2 | 14× (below own 2026 low; a pure distributor with negative FCF) | **₹437** | **−60%** |
| Base | 3,246 | 2.4% | 68.5 | ₹45.1 | 20× (middle of own 2026 range of 16–21×) | **₹902** | **−18%** |
| Bull | 3,516 | 2.8% | 86.6 | ₹56.9 | 28× (brand re-rating plus cash fixed) | **₹1,594** | **+44%** |

*Arithmetic via `valuation_calc.py`.*

## Step 4: Section B — multiple re-rating on Base EPS (₹45.1)

| Multiple | Basis | Target | Gap |
|---|---|---|---|
| 14× | Distributor de-rating | ₹631 | −43% |
| 20× | Own 2026 middle | ₹902 | −18% |
| 25× | Today's TTM multiple held | ₹1,128 | +2% |
| 28× | Brand-led re-rating | ₹1,263 | +14% |

The market is currently paying ~25× for Base-case earnings. **Most of the Bull case is multiple, not earnings.**

## Step 5: Cross-check — EV/EBITDA
- Base FY27 EBITDA ≈ ₹127 cr (3.9% margin on ₹3,246 cr).
- At 12× that gives an EV of ₹1,519 cr. Less net debt ₹302 cr and NCI ≈ ₹24 cr gives equity ≈ ₹1,193 cr, or **≈ ₹784/share (−29%)**.
- The current ~17× EV/EBITDA is a brand-company multiple applied to a group where ~86% of revenue is distribution.

## Step 6: Part evaluation (SOTP)
- **Brand (SCL, HK):** FY26 PAT ₹37.4 cr × 77.5% = ₹29.0 cr to CNL. At 30× that is ₹870 cr. The 30× is the level an analyst suggested on the May-26 call for branded businesses ("30, 40x", an analyst's figure). The multiple is **not** discounted here, even though SCL is not audited by the group auditor and carries an undisclosed licence-renewal risk.
- **Market Entry + parent:** owners' PAT ₹61.9 cr − ₹29.0 cr = ₹32.9 cr. At 12× that is ₹395 cr.
- **SOTP ≈ ₹1,265 cr → ₹842/share (−24%).** Debt is already reflected, because PAT is after interest.
- Even crediting the brand with a premium multiple and ignoring a holding-company discount, the parts add up to less than the current price.

## Step 7: Scoreboard

| Scenario | Method | Target | Gap | What has to be true |
|---|---|---|---|---|
| Bear | P/E 14× | ₹437 | −60% | Middle East halves brand exports; credit tightening slows growth; interest keeps rising |
| Base | P/E 20× | ₹902 | −18% | 20% growth, margins flat-to-down, cash still weak |
| Base (hold multiple) | P/E 25× | ₹1,128 | +2% | Market keeps paying today's multiple |
| SOTP | P/E by part | ₹842 | −24% | Brand at 30×, distribution at 12× |
| EV/EBITDA | 12× | ₹784 | −29% | Distribution-style EV multiple |
| Bull | P/E 28× | ₹1,594 | +44% | Guidance delivered **and** receivables normalise **and** Honeywell renews |

**Verdict:**
- The risk/reward is **unfavourable**: roughly −20% to −60% of downside against +44% in a Bull case that needs every open item to resolve.
- The Base case is the most likely path: revenue delivered, margins and cash not. The biggest swing factor is the multiple. Sections A and B agree that at ~25× the stock already prices in more than the Base-case earnings support.
- **The cash question is the most important point.** CNL generated −₹272 cr of operating cash flow in FY26 and −₹278 cr over three years, against ₹172 cr of reported PAT. Every earnings-multiple target above is a statement about *accounting* profit. Until receivables convert, none of that profit has reached shareholders as cash.

## Sources
- **Annual reports:** AR FY26 (consolidated statements, note 23B geography, note 37 segments, AOC-1, standalone note 36 related parties, Directors' Report item 35); AR FY25; AR FY24.
- **Decks:** Q1 FY27 deck (4-Aug-2026); Q3 FY26 deck (5-Feb-2026).
- **Calls:** 16-May-2025, 12-Nov-2025, 15-May-2026 (page numbers from printed footers).
- **Ratings:** CRISIL rationales of 4-Dec-2025 and 6-Aug-2026.
- **CMP:** bajajfinserv.in/investments/cnl-share-price (29-Sep-2026 15:29 IST); cross-checked against icicidirect (₹1,097.70 close, 29-Sep) and tickertape (₹1,098.20, 25-Sep). Historical P/E points: in.investing.com (₹670.20, 14-May-2026) and share.market (TTM P/E 20.68, 13-Jul-2026).

*Research only. Not investment advice.*
