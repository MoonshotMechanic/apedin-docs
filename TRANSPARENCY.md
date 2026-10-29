# Transparency

Document prepared: **23 October 2026**. Individual assessment dates below describe when that work happened, not a fresh scan of the current service.

## What apedin does

apedin presents attributed meme-coin callouts, public source activity and community discussion. Supported sources include Pump, FOMO, GMGN and Axiom. Available records and context differ across those sources.

The current service does not execute trades or take custody of funds. Wallet connections are used for supported identity and account features; they are not permission to transfer assets. apedin support does not need your recovery phrase or private key.

## Data coverage and interpretation

- **The feed is an observed dataset.** It is not a complete archive of every call, trader or market event. Collection start dates, interruptions and available history differ by source.
- **Pump collection starting point.** Pump background engagement collection starts with a one-time 24-hour lookback. Refresh jobs from before that fixed starting point are excluded; later work remains as it ages. Stored calls and existing XP awards remain. This is not a rolling data-retention limit.
- **Ranked refresh scope.** Background history and engagement refreshes focus on ranked/KOL identities. Live discovery and limited identity checks remain broader; existing records and XP awards are retained. Leaderboard delays, source limits and outages can still leave gaps. Non-ranked profile and engagement data may stop refreshing.
- **Timing varies.** Posts, captures, refreshes and market snapshots can have different timestamps. Provider delays, browser-assisted collection and outages can affect freshness and completeness.
- **Coin-age fallback has limited coverage.** Newly received supported Solana calls with a missing age can enter a bounded lookup queue. This fallback accepts a creation date only after checking that a matching finalized transaction initialized the exact mint. Provider availability, verification and queue limits can delay or prevent an age from appearing. Call time, first-seen time and trading-pair age are not substituted for coin creation.
- **Source attribution matters.** Imported records remain associated with their source. Similar names or contextual links do not prove that two accounts have the same owner.
- **Researched connections are dated evidence.** Public trader pages can show source-linked or confirmed public connections. These labels do not establish proof of control, merge trading histories, or grant ownership or XP. Unresolved research leads and referral links are not presented as confirmed trading accounts. Research links can expire or be removed; use the profile’s correction-support link if a connection is wrong.
- **Public pages and indexing differ.** Supported source accounts can have public pages while sparse pages remain excluded from search indexing. Eligible pages enter the sitemap, but search engines decide whether to index them.
- **Profile claims have a separate boundary.** A claim or verified connection reflects the stated identity-check scope. It is not an endorsement, proof of legal identity or a financial qualification.
- **Metrics need context.** Prices, market caps, holder counts and positions can be provider-reported snapshots. They are not independently verified entry prices, realised returns or promises of future performance.
- **Other ranked mentions use captured history.** Feed-row counts refer to other currently ranked/KOL source accounts recorded mentioning the same token. Repeat mentions from one source account count once, the row’s caller is excluded, and the detail list shows each account’s latest recorded mention. Accounts on different platforms are counted separately; this is not a count of independently verified people or a complete record of every mention.
- **Attention measures observed activity.** Experimental Attention indicators are not price predictions or token safety scores. Missing coverage should be interpreted as unavailable information, not zero activity.
- **Progression is service recognition.** XP, levels, badges and evolution are not money, an entitlement to a token, or evidence of investment skill.

An integration or source label does not imply a partnership or endorsement by that provider. Linked platforms have their own terms and policies.

## Accounts, privacy and moderation

Browsing the feed does not require an account. Participation features require sign-in. Imported public information may concern people who have never registered with apedin.

Our [Privacy Policy](https://apedin.family/privacy) explains information handling and requests for access, correction or removal. Our [Terms of Use](https://apedin.family/terms) explain participation, content and account rules. Those policies remain the primary documents for those subjects.

Use [apedinfamily@outlook.com](mailto:apedinfamily@outlook.com) for account, privacy and content concerns. Please keep personal information out of public reports.

## Security review evidence

### Internal engineering review — 13 October 2026

An internal engineering review covered local application code, authentication and authorisation, public API inputs, image uploads, browser rendering, an operator-side ingestion bridge, dependencies and container packaging.

The review recorded dependency updates and targeted fixes, along with local automated tests and packaging checks. At the time, the pinned Python dependency scan reported no known advisories. JavaScript dependency advisories remained in upstream wallet-related dependency chains; the review did not establish that all were exploitable through apedin, or that they could all be dismissed.

This was a targeted engineering review, **not an independent third-party penetration test or security certification**. Its local checks did not establish end-to-end production security, and its dependency results are historical. Changes since then are outside that review's coverage. No independent third-party penetration-test report is published in this repository.

### Reading future assessment summaries

Assessment summaries should state their date, reviewed version or scope, method, material outcomes and limitations. Automated scans, AI-assisted reviews, internal manual reviews and independent assessments should be labelled distinctly. A passing test suite or a clean dependency scan is not an audit of the whole service.

Sensitive reproduction details, personal information and internal operational logs do not belong in public summaries. Suspected vulnerabilities should follow our [private reporting process](SECURITY.md).

## Release information

The [changelog](CHANGELOG.md) records selected shipped milestones. Unreleased work and local test results are not evidence that a change is running in production. The website footer identifies the running release.

This repository contains public documentation; application code and deployment systems are maintained privately. Keeping code private limits what readers can independently verify from this repository, so claims here should be read within the stated evidence and scope.

## Captured X activity

X activity is a captured snapshot of a direct post associated with a coin, not a live growth meter. For supported Solana Token-2022 coins with self-referenced metadata and a public HTTPS metadata file, apedin reads the coin’s own X link; text in a feed call is not used as that source. Unsupported metadata or a missing X link can leave X activity unavailable. Supported immutable IPFS metadata can use a fallback gateway after verifying the content against its original identifier. Temporary metadata lookup failures receive bounded retries; this can delay an X indicator after a call appears. An invalid metadata update does not substitute an arbitrary post; previously verified evidence can remain marked stale while it is rechecked. Feed calls about the exact same token address and chain can share a captured post snapshot selected by the coin’s current verified link; earlier captures remain preserved. The card identifies coin-level evidence, the X post author and actual capture time. These are not metrics at the displayed call’s time, and the displayed caller is not assumed to have authored or endorsed the post.

Replies, likes, views, reposts and quotes are provider-reported observations. Missing values remain unavailable. Author details provide context, not a credibility or safety rating. A newly received call may link an older post; the card shows the post age at capture.

Comparative scores remain unavailable without eligible reference data. New snapshots use the experimental Post activity score, comparing previously captured posts of similar post age: views 35%, replies 25%, likes 20%, smoothed interaction rate 15%, and account age 5%. Account-age credit stops increasing after two years. Scores below 100 views are reduced by a low-view safeguard; missing components remain explicitly uncertain. Views and account age may contribute even when replies and likes are zero. These are chosen product settings, not statistically proven accuracy or confidence probabilities. Earlier Post engagement scores remain frozen under their original formula. Future calibration does not rewrite earlier snapshots or scores. These indicators do not measure bots, authenticity, sentiment or expected investment returns.

Collection is limited to new incoming calls, bounded to at most 1,000 unique post attempts per UTC day, and does not refresh for each viewer. Budget-excess links can be skipped rather than collected later, so coverage is incomplete. No historical demonstration data is used to seed production results.

## Compact caller previews

Selecting a feed-row avatar opens a compact caller preview. It can show an available source rank and the row’s recorded position snapshot, when supplied by that source. These are source-labelled, call-scoped observations, not a caller-wide performance claim. The preview opens the existing caller profile for more context.
