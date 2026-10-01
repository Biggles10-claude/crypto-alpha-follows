# Sources — searches, URLs, and verification surfaces

Audit date: **2026-10-02** (Australia/Perth / AWST).  
Method: multi-source seed → per-handle verification (TwitterScore + secondary) → confidence tagging → reject log.

## Primary user context

- Existing education/quality follows (dedupe baseline): https://biggles10-claude.github.io/crypto-quality-follows/

## Web searches used (representative)

- `crypto twitter alpha accounts 2025 2026 on-chain analysts deal flow`
- `best on-chain analysts twitter crypto whale trackers 2025 2026`
- `Legion Echo Sonar crypto community sale Twitter accounts deal flow 2025 2026`
- `best crypto researchers twitter CT independent theses DefiIgnas 0xFinish`
- `crypto twitter memecoin launch hunters on-chain process Ansem Murad accounts 2025`
- `crypto twitter scam hunters security researchers mid size accounts 2025 2026`
- `crypto twitter token unlock tracker accounts VestLab TokenUnlocks analysts`
- `best Dune Analytics analysts twitter crypto researchers mid size`
- `Australian crypto twitter alpha traders researchers APAC Asia session 2025 2026`
- `Echo Cobie crypto angels twitter accounts early deals community sales radar`
- `"crypto twitter" "must follow" OR "alpha accounts" researchers mid 2025 OR 2026`
- Handle-specific TwitterScore / reputation queries for EmberCN, Hsaka, Taiki, ScamSniffer, StalkHQ, GLC, ilemi, etc.

## Roundup / article URLs fetched or cited

- https://captainaltcoin.com/10-must-follow-crypto-analysts-on-x-twitter/
- https://airdropalert.com/blogs/list-crypto-x-accounts/
- https://www.valueassets.net/the-ultimate-list-of-must-follow-crypto-x-accounts-in-2026/
- https://cointracking.info/blog/37-company-accounts-to-follow-crypto-twitter/
- https://threadreaderapp.com/thread/1704569023067996646.html (ardizor Tier-1 fund follows method)
- https://echo.xyz/investor/sonar.html
- https://echo.xyz/
- https://legion.cc/
- https://www.cryptotimes.io/2025/10/21/coinbase-bets-on-ico-comeback-with-375-million-echo-deal/
- https://glcresearch.xyz/ / https://glcresearch.xyz/announcing-hrc-the-research-hub-for-hyperliquid/
- https://tokenomist.ai/
- https://cointelegraph.com/news/zachxbt-slams-crypto-influencer-over-memecoin-promotions
- https://bitquery.io/investigations/ansem-black-bull-370x-investigation
- https://www.ledger.com/academy/topics/crypto/how-to-track-crypto-whale-movements
- Buzzberg speaker pages (threadguy / x256xx) — used only as “people track calls” evidence, not as truth.

## Per-handle verification surface

Primary: **https://twitterscore.io/twitter/{handle}/** for follower band, bio, about-blurb, rename notes, and smart-follower context.

Examples verified this way (non-exhaustive):  
`EmberCN`, `loomdart`, `HsakaTrades`, `TaikiMaeda2`, `realScamSniffer`, `waleswoosh`, `0xSisyphus`, `GLC_Research`, `andrewhong5297`, `StalkHQ`, `knowerofmarkets`, `echodotxyz`, `legiondotcc`, `cobie`, `Rewkang`, `ai_9684xtpa`, `hildobby`, `adamscochran`, `icobeast`, `PeckShieldAlert`, `SlowMist_Team`, `immunefi`, `pcaversaccio`, `officer_secret`, `MetaSleuth`, `MistTrack_io`, `cryptoquant_com`, `aixbt_agent`, `notthreadguy`, `WuBlockchain`, `mrjasonchoi`, `FourPillarsFP`, `Jonasoeth`, `thedefivillain`, `0xFinish`, `RugDocIO`, `GoPlusSecurity`, `BlockSecTeam`, `SEAL_911`, `coffeebreak_YT`, `Token_Unlocks`, `x256xx`, `hupzy_agent`, `stablemark_`, `gainzy222`, `awawat`, `DegenSpartan`, `FrankieIsLost`, `_charlienoyes`, `ZeMariaMacedo`, `scupytrooples`, `CL207`, `CryptoCred`, `DonAlt`, `DaanCrypto`, `GCRClassic`, `0x_b1`, `Adam_Tehc`, `0xBoxer`, `kyoronut`, `nico_mnbl`, `transmissions11`, `SantimentData`, and others listed in `accounts.json`.

Secondary: Thread Reader App, Rattibha, TwStalker/Tweetlook mirrors, project docs, GitHub (SEAL 911), Substack (Thor Hartvigsen — handle unresolved).

## Verification blockers

1. **X.com / x.com** — automated fetch frequently blocked or empty; not used as sole source of truth.
2. **Nitter / xcancel** — inconsistent availability; not relied on for bulk verification this pass.
3. **TwitterScore rate / empty “Detail” pages** — some handles returned empty shells (`ThorHartvigsen` 404, `Coffeezilla` wrong slug → corrected to `coffeebreak_YT`, `TraderSZ`/`PC_Larp`/`VestLab` weak).
4. **Follower counts** — approximate bands from TwitterScore “as of October 2026” text; expect drift.
5. **Renames** — Spot On Chain → Hupzy; TokenUnlocks → Tokenomist/`Token_Unlocks`; Beast_ico → icobeast; officer_cia → officer_secret. Always re-check live.

## Output files

- `ACCOUNTS.md` — human table + honesty + starter pack
- `accounts.json` — machine-readable array
- `REJECTS.md` — this audit’s exclusions
- `SOURCES.md` — this file
