# Changelog

## 0.29.3 — 2026-10-28

- Redesign standalone public profiles with layered surfaces, recessed rank displays, and clearer calls, identity and evidence sections. In-feed profile drawers retain their existing layout.
- Show immediate posting feedback and explicit confirmation for comments, clear confirmed drafts, and prevent duplicate taps while posting.
- Simplify feed timestamps by removing the Replayed label.
- Prepare an optional independently verified Solana coin-age fallback; it remains disabled pending production activation.

## 0.29.2 — 2026-10-28

- Fix comments on certain Axiom calls whose post identifiers contain a source prefix.
- Keep the page at its normal size after focusing a comment field on mobile.

## 0.29.1 — 2026-10-27

- Refresh available verified coin-creation dates more frequently and deliver late results sooner while keeping new feed rows prioritized.
- Preserve verified dates and leave unknown ages blank; call times and trading-pair ages are not substituted for coin creation.

## 0.29.0 — 2026-10-27

- Reorder ultra-compact rows to show avatar, rank, source, time and username; shorten position labels.
- Remove the Observations page.
- Give thesis text a separate section with available caller avatar/ranks, keeping market capture details below.
- Use clearer experimental X engagement wording; scoring weights and frozen evidence stay unchanged.
- Add a coin-age filter to the current ticker results, with stacked selectors and aligned navigation. Unknown coin ages remain visible under All ages; trading-pair age is not substituted.
- Reduce reward-processing work that can delay feed requests while preserving ownership and reward eligibility checks.
- Improve release preflight checks for available storage.

## 0.28.6 — 2026-10-27

- Improve X metadata processing throughput and share queued work across repeated calls for the same coin.
- Preserve one captured snapshot per post, forward-only collection and the existing daily collection limit.

## 2026-10-27 — KolScan ranking recovery

- Restore fresh daily, weekly and monthly KolScan rankings after adapting to its updated leaderboard response.
- Rank badges continue to require current supporting evidence; expired rankings are not presented as current.

## 0.28.5 — 2026-10-26

- Recover supported IPFS-hosted coin metadata through a content-verified fallback when its original gateway is unavailable.
- Retry temporary coin-metadata lookup failures within bounded limits; previously captured X snapshots stay unchanged.
- Expand the desktop feed into the available page width while retaining the sidebars and mobile layout.

## 0.28.4 — 2026-10-26

- Resolve a supported Solana Token-2022 coin’s own X link from self-referenced on-chain metadata and a public HTTPS metadata file, rather than from text in a feed call. Unavailable or invalid metadata is never replaced with an arbitrary post.
- Keep coin-level X evidence compact: the preview shows captured metrics and post context, while source provenance and calibration context remain available in the expanded details.
- Open a compact caller snapshot from a feed-row avatar. It shows available source rank and the row’s recorded snapshot, then opens the existing caller profile when selected. Desktop supports hover; touch devices support tap.

## 0.28.3 — 2026-10-26

- Show an existing captured X snapshot on feed calls about the same token and chain, even when a different call supplied the post link.
- Identify coin-level X evidence separately from the feed caller, with post attribution, source context, and capture time. Snapshot metrics are not historical metrics at the call’s time.

## 0.28.2 — 2026-10-26

- Improve restoration of a previous sign-in when the same account remains authenticated with the sign-in provider. Signing out suppresses automatic restoration.
- Show newly captured X evidence on existing feed rows without a page reload.
- Add compact X activity indicators and a detailed hover/tap card where a captured post snapshot is available. Mobile uses a bottom card.
- Begin forward-only collection of direct X post links in newly arriving feed calls. Historical feed records are not backfilled. Each post has one captured baseline, with capture time and provisional status shown.


Selected shipped milestones, written for people using apedin. This is not an exhaustive record of every patch or deployment. The website footer displays the running application version; the newest entry below should not be treated as a live version check.

Release dates below follow the existing product release records.

## 0.27.3 — 2026-10-26

- Highlight and reveal the selected thesis timeline post; use the newest post when the requested post is unavailable.

- Offer Save or share image on devices supporting native image sharing, with Download image kept as a fallback.

- Use more of the existing rank-badge width for larger rank numbers, retaining badge and feed-row heights.
- Enlarge compact-feed names, source marks, activity metrics and primary action icons within their existing layout.
- Grey out profile video entry points while video creation is unavailable.
- Keep the history pause button’s accessibility state aligned with its Resume live label.

## 0.27.2 — 2026-10-25

- Fix an error that could leave a caller profile drawer blank.
- Show explicit loading placeholders while sign-in options and other ranked mentions load.
- Make thesis links clearer with visible actions and keyboard focus treatment.
- Point site documentation links to the new public documentation repository.
- Keep video creation visibly disabled when rendering is unavailable.
- Load compressed share-card artwork only as each style is selected.

- Share text includes the caller’s available source rank and ranking period, including the X post shortcut.

- Larger token artwork and names accompany a prominent source-and-rank identity panel with a raised badge, larger rank label, and platform icons beside source names. Rank remains conditional on available source data.

- Image cards now use angled, dimensional amount lettering and compact raised return badges; positive returns remain emerald and negative returns red.

- Choose Gold Standard, Profit Ticket or Night Signal for an individual callout image.
- Larger caller names adapt to available space, with source and rank shown where available.
- Positive position returns use emerald green; negative returns use red. Cards retain a captured-snapshot label and omit the since-call line.

## 0.27.1 — 2026-10-25

- Refresh historical counters separately from live status, with clear warming and stale states.
- Reduce avoidable work when loading activity statistics and token context.
- Use smaller homepage images and fonts and defer styles for secondary interfaces.
- Remove the Scout saved-research promo, retain saved calls, and add the Telegram channel to footer links.
- Add recognisable icons to email, Apple, Telegram and Discord sign-in options.

Deployed and checked live. Sampled status, activity statistics and ranked-feed responses improved; response times vary with traffic and workload.

## 0.27.0 — 2026-10-24

- Add optional founding-member invite codes and shareable signup links. Signup remains free; a code adds founding-member status, not ownership verification, XP or paid access.
- Add profile-video previews using supported, source-labelled performance snapshots. Available periods and figures depend on the source; unsupported results are omitted. MP4 downloads are not available yet.
- Add an animated Tension Ribbon for market sentiment, alongside a separate captured call-activity rate. Reduced-motion preferences are respected.
- Add Good Calls to profile histories, showing positive recorded source P/L snapshots rather than live or independently verified returns. The full Calls history remains available.
- Simplify public profile backgrounds and improve performance-badge readability.
- Reduce image download sizes, align browser cache keys, improve feed accessibility labels, and reduce unnecessary work when building profile sitemaps.

## Additional sign-in options — 2026-10-24

- Enable Apple, Discord and Telegram under **More ways to join**, with successful sign-in continuing to optional profile setup.

## 0.26.0 — 2026-10-24

- Add optional, resumable profile onboarding with public social links and multiple self-added trading profiles. Keep available sign-in options limited to providers enabled for the live site.

- Add a guest preview with three readable fresh calls, locked leading ticker cards, and grayed token rooms; signing in unlocks the full interface.

- Reduce memory peaks while processing imported profile pictures and token icons.

- Remove standalone platform referral panels from profiles and token details; retain referral attribution on supported existing destination links.

## Reliability update — 2026-10-24

- Restore site access after a connection interruption and add automatic recovery when an application restart leaves its public connection stale.

## Email branding — 2026-10-24

- Set the sign-in email brand name to **apedin.family**.

## 0.25.2 — 2026-10-24

- Clarify that referral buttons open platform signup or landing pages, keep trader profile links separate, and label Axiom handle links as landing links rather than verified profile URLs.

## 0.25.1 — 2026-10-23

- Keep previously served profile and token images available during background refreshes, within bounded cache storage, so existing pages continue to display them.

## 0.25.0 — 2026-10-23

- Align normal and compact feed cards beside an avatar/rank column, with larger clickable source badges, three visible badges plus overflow, and only current confirmed connections included in additional ranks.

- Add disclosed platform referral links, with optional member-owned links on their own or approved-claimed profiles; keep account evidence and referral destinations separate.

- Enrich in-app trader profiles from exact source-account research independently of public-page eligibility, keeping uncertain links separate and source snapshots dated.

- Add reserved, readable main trader profile addresses, with confirmed trading accounts shown separately and existing source links preserved.

- Add a neutral Graphite default profile banner with a subtle public profile address.

- Cache imported profile pictures and token icons as local thumbnails, with background refresh and local placeholders; callout attachments retain their existing behavior.
- Show profile-picture upload and removal feedback beside the picture controls, including file validation errors.
- Hide ranked discovery sorting controls in Following and Saved; Hot and Rising remain scoped to ranked/KOL activity.
- Present supported profile links as compact header icons with overflow, and use platform marks on source ranking chips while retaining connection evidence.
- Refine the Everyone coming-soon panel with clearer typography, concise copy, and a styled ranked-feed action.
- Improve desktop token-strip text within the original card dimensions, preserving mobile sizing and containing long names.
- Require sign-in to save calls or research notes. Saved content remains local to the browser.

- Use readable, stable trader profile addresses with redirects from older links.
- Copy public trader profile links directly from the profile drawer.

## 0.24.0 — 2026-10-23

- Complete the Atlas public profile design with artwork, clearer activity sections and account-specific totals.
- Add a browsable trader directory and improve public profile search and sharing metadata. Sparse profiles remain excluded from indexing.
- Focus Hot/Rising discovery on ranked/KOL activity and token timelines on eligible ranked/KOL accounts and Apedin members.
- Improve Pump history refresh scheduling and hide confirmed-empty other-caller badges.

## 0.23.0 — 2026-10-23

- Add public pages for supported imported trader profiles, with source-specific captured activity and links back to the interactive profile drawer.
- Refresh public profile and drawer layouts and show researched connections with evidence labels and check dates.
- Keep research links separate from ownership verification, account permissions and XP. Unresolved identity leads remain unpublished; sparse profiles are excluded from search indexing.

## 0.22.4 — 2026-10-23

- Rename Prestige to Evolution across progression labels and use E 0–E 10 for avatar badges. Levels, XP and earned artwork are unchanged.

## 0.22.3 — 2026-10-22

- Replace feed-row Attention charts with counts of other currently ranked/KOL source accounts that mentioned the same token. Open the count to see each account’s latest recorded mention, time and available source links; repeated mentions count once per source account.
- Keep ticker Attention available and clarify ranked refresh coverage in Settings, filters, alerts and activity descriptions.
- Improve Ranked search and reduce database contention while retaining stored history and collection scope.

## 0.22.2 — 2026-10-22

- Reduced memory overhead for Attention history and public statistics while preserving chart observations, stored records and collection coverage.

## 0.22.1 — 2026-10-22

- Put Ranked first and keep it as the default view. Everyone opens a dedicated message panel while broad profile coverage is unavailable.
- Start Pump background engagement collection with a one-time 24-hour lookback, then retain subsequent work as it ages. Existing call history and XP awards are retained.

## 0.22.0 — 2026-10-22

- Focused background history and engagement refreshes on ranked/KOL callers while keeping live discovery active.
- Preserved existing history, XP awards, sign-up and community participation.
- Added recovery for newly ranked callers and clearer freshness and queue coverage reporting.

## 0.21.5 — 2026-10-22

- Made Ranked the default feed and preserved that preference for returning visitors.
- Marked the Everyone feed as temporarily unavailable while keeping sign-up available.
- Improved live-feed behavior during rate-limit cooldowns.

## 0.21.4 — 2026-10-22

- Added public footer links and updated the support contact details.
- Improved sign-in loading so it remains stable while account services initialise.

## 0.21.3 — 2026-10-22

- Reuse the validated release build and add a production-sized resource rehearsal before rollout. Keep fresh pre-release backups and scheduled restore checks.

## 0.21.2 — 2026-10-22

- Added the experimental Observations page, summarising caller market-cap habits and overlapping community participation from recorded calls.
- Observations refreshes daily from completed UTC days and shows its date range, sample sizes and most recent update status.

## 0.20.1 — 2026-10-20

- Refreshed browser assets so returning visitors receive the updated ticker history, mobile drawer handle and stream metrics.

## 0.20.0 — 2026-10-20

- Added experimental Attention history bars, with activity-based wording and gaps when observations are unavailable.
- Added a one-minute token ranking window.
- Added a mobile drawer handle for tap or drag-down dismissal.
- Expanded stream cards with attention, holder counts, call totals and token or trading-pair age.

## 0.19.0 — 2026-10-20

- Added landscape and portrait stream overlays, including explicit demo and unavailable-data states.
- Improved source-rank badges and text-size controls in the ultra-compact feed.
- Gave Attention labels their own space to avoid overlap with market data.

## 0.18.0 — 2026-10-20

- Added public member profile pages with individual page metadata.
- Added a member directory and sitemap for eligible profiles.
- Made public profile links usable in a new tab and without JavaScript.

## 0.17.0 — 2026-10-20

- Added signed-in token-room discussion and replies to individual calls.
- Added captured thesis histories and market snapshots for new posts, without inventing historical prices.
- Improved token identification, missing artwork and holder context.
- Clarified Attention explanations and missing-data states.

## 0.14.1 — 2026-10-19

- Released automatic prestige progression and updated weighting for qualifying external activity.
- Added brushed-copper Prestige 2 presentation and clearer profile level labels.
- Improved release-backup reliability.

## 0.10.1 — 2026-10-18

- Expanded the profile hub, source-linked histories and mobile profile layout.
- Improved evidence-based profile connections and ownership-claim handling.
- Corrected duplicate-ingestion and slow linked-history behaviour.
