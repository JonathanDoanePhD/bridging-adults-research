# Bridging adults: what eleven projects found together

> Exploratory research on public data. Every figure and citation needs checking against
> its original source before it appears in funder reports, grant applications or public
> material. Associations, not causal effects, unless stated.

## The through-line

**Places, schools and young people do better where relationships cross class lines, and
access to those relationships is most unequal exactly where they would matter most.**
Mentoring is one deliberate way to build them. To show that it works, a program has to
measure confidence and connection separately, plan for small effects, and protect its
comparison group from dropping out.

## 1. Where (Project 01: Opportunity & Mobility Atlas)

- **Cross-class friendship is the strongest single correlate of upward mobility.** Across
  ~3,000 counties, children from low-income families earn **+2.7 income percentiles more as
  adults** per SD of economic connectedness. That holds within states and after adjusting
  for 14 other traits, and it alone predicts 39% of the variation in states the model never
  saw.
- **Youth-nonprofit density shows no relationship with mobility** once other traits are
  known. *Having organizations* is not the same as *building connections*.
- **124 high-need, low-supply counties** (64 with at least 2,000 children). They do worse
  than their disadvantage predicts (85% below prediction) and are low on cross-class
  friendship. **315 high-poverty counties "beat the odds"**, many near the priority counties,
  as possible places to learn from.
- Explore: `https://github.com/JonathanDoanePhD/opportunity-mobility-atlas/blob/main/output/atlas_explorer.html`.

## 2. Why (Project 02: Mathematics of Mentorship)

| Finding | Data | Implication |
|---|---|---|
| 80% of children below the poverty line have a non-parental adult to rely on, vs. 94% above 400% FPL; activities explain about a third of the gap | NSCH 2024 | Access is the first outcome to move |
| Such an adult goes with +14 pts flourishing, +12 school engagement, +6.5 hope | NSCH 2024 | Supportive adults matter broadly |
| Engagement benefits are larger for high-adversity youth; hope benefits are *smaller* for low-income youth | NSCH 2024 | School-related outcomes: compensation. Emotional outcomes: hardship dampens |
| Schools where lower-income students befriend higher-income peers graduate more disadvantaged students, **4x more so in mixed schools** | Social Capital Atlas + EDFacts (8,934 schools) | Bridging matters beyond exposure |
| Belonging goes with better grades and less hopelessness, but less so under hardship | YRBS 2023 | Belonging is a wellbeing outcome |
| Supportive teachers → self-efficacy (directly) → achievement carries most of the link; belonging is a separate channel. Holds in all 65 PISA systems; no confidence penalty for disadvantaged students in mixed schools | PISA 2022 | Build confidence (mastery, encouragement) for school outcomes; connection for wellbeing |

**Revised model:** supportive/bridging adults → **self-efficacy** → school outcomes, and →
**belonging** → wellbeing. Hardship dampens the emotional channel; anxiety is the largest
drag on self-efficacy.

## 3. How we'd know (Project 03: Mentorship Impact Engine)

- A 29-item youth survey (plus one pilot stress item). A third of the items reuse national wording, so programs get free
  benchmarks: participants at intake vs. NSCH and YRBS teens by income or hardship.
- A synthetic-data simulator, analysis pipeline and dashboard, with privacy built in
  (pseudonymous IDs, restricted fields kept separate, small groups suppressed, people make
  every decision).
- **What building it taught us:**
  - Comparing everyone assigned to the program, plus measurement error, shrinks a true
    0.20-0.25 SD benefit to about **0.07-0.16 SD measured**.
  - That needs **~400 youth per group** for 80% power at 0.2 SD.
  - **Uneven dropout between groups** is the biggest threat.
  - **Early match closures** erase gains.
  - **Short mixed-format scales** are fragile.

## 4. Round 2: the same question at other points

| Project | Finding | What it adds |
|---|---|---|
| **04 College Bridges** | 1980s college success rates still track today's low-income earnings (rank r = 0.85). Low-income students rise further at colleges with more high-income classmates (+5.6 pts per SD within selectivity tier), but **friending bias shows no link at college**. 52 of 64 priority counties have no affordable, high-mobility college within 60 miles | Bridging matters most *before* college (high school, Project 02); after that, access to mixed, well-resourced campuses matters, and priority counties lack them |
| **05 Who's Around** | Low-income teens spend **8 fewer minutes a day** with non-family adults outside school and work (about 50 hours a year), and more with extended family and screens. Sports and volunteering supply much of the gap | The access gap in minutes; **one hour a week of mentoring is about the size of the gap** |
| **06 Adults in the Building** | Counselors per student are flat across school poverty while chronic absence doubles (1.7 vs. 3.7 support staff per 100 chronically absent students). Snapshots mislead (staff go where need is); **adding counselors showed no detectable change in chronic absence** over two years | Spreading general staff thinner isn't a quick lever; a consistent personal relationship is different and needs its own evaluation |
| **07 Return on Mentoring** | At $2,000 per participant, a program breaks even if it adds **~1 high school graduate per 100 participants** (2 at a 7% discount rate). Each extra graduate is worth about $204,000 in lifetime earnings; about a quarter of benefits return as taxes | The bar for a positive return is low, but the effect on graduation is the unknown, so linking to graduation records is the key evaluation step |
| **08 Mentoring Evidence Engine** | Agents screened 9,138 ERIC abstracts and double-coded 935 youth mentoring studies (design kappa 0.91). **The stronger the study, the weaker the result:** 84% of findings are positive at rigor 1-2 but 56% at rigor 4-5. Credible academic effects are about d = 0.1-0.27. Only 14 randomized trials report graduation, and the K-12 ones are mostly null. **Bridging programs stay more positive within rigor bands** (79% vs 52% at rigor 4-5; 16 studies, so a lead, not a conclusion) | Confirms 03's small-effect planning and 07's 0-4 point graduation range; the field rarely reports dose or format, and the best-supported lever is the bridging one this portfolio centers on |
| **09 Federal Youth Program Investment Map** | Agents tagged 2,974 NSF youth STEM awards ($3.39B, 2014-24) and 390 OJJDP mentoring grants ($1.04B). **AI-focused awards rose from 2% to 21%; mentoring stayed at ~14% (3% central) and bridging at 13%.** Planned rigorous evaluations fell from 17% to 8%. The highest-need county fifth gets **0.46x its per-child share** of NSF youth STEM money (college-access programs: 1.40x), and the 124 priority counties are nearly absent. 79% of federal mentoring money goes through national intermediaries. Of 2021-24 awards, 20% were terminated in 2025, but 45-56% of those naming Black, Hispanic, Native youth or girls (2.5% naming no group) | Federal STEM investment is not reaching the places 01 flags, and it rarely funds the bridging relationships 02-08 point to; a pilot in priority counties fills a real gap but cannot count on federal STEM streams |
| **10 Nonprofit Program DNA** | Agents tagged the Form 990 program text of 15,473 youth, education, recreation and human-services nonprofits. **12.7% of youth development organizations describe mentoring, about five times the 2.3% coded as mentoring by the IRS; 89% of mentoring is uncoded.** Mentoring organizations are ten times as likely to bridge (21% vs 2%). Evidence is thin (1.3% report numbered outcomes). Only 4 of 124 priority counties have a filing mentoring organization in the county (62 with neighbors) | Fixes 01's weakest input: mentoring supply is larger nationally than the codes show, but not in priority counties, where a pilot would mostly start from scratch or partner across county lines; 136 candidate partners for community review |
| **11 AI and the Opportunity Ladder** | Agents rated all 18,797 O*NET tasks (reference-model weighted kappa 0.78-0.90; r = 0.80 with published human exposure labels across 923 occupations). **AI can do much of 39% of jobs needing a bachelor's but 19% of jobs entered without one; 63% of no-BA jobs are human-anchored.** The exception is the office first rung: about 17M no-BA jobs (customer service, admin assistants, clerks, receptionists, bookkeeping) are mostly AI-doable. 89 of 137 no-BA occupations paying the median or more are human-anchored (trades, allied health, utilities, public safety), reachable through certificates paying Pell completers $50-69K. Priority counties' jobs are less AI-exposed (30% vs 35%) | Mentoring should steer youth toward human-anchored credentials and treat office entry jobs as stepping stones; bridging ties to people in trades and allied health are the scarce resource |

## What this suggests for a pilot

1. **Where:** start from the Atlas priority list, then have people who know those
   communities check it. Look at nearby beat-the-odds counties for partners to learn from.
2. **What:** mentoring that deliberately bridges (introductions to people and
   opportunities), builds confidence through mastery experiences, and pairs with practical
   supports where hardship is high.
3. **Dose:** about one hour a week of mentoring matches the daily gap in time with non-family
   adults (05). Use sports, volunteering and work-based activities as settings (05).
4. **After high school:** build college navigation into the program, since most priority
   counties are far from bridge colleges (04).
5. **How to evaluate:** use a lottery when oversubscribed. The literature (08) shows weak
   designs overstate effects, so a rigorous design is what will make results believable. Link to graduation records (with
   consent) so the return calculator (07) can use a measured effect. Primary outcomes are belonging,
   self-efficacy and engagement; access outcomes are supportive adults and bridging ties.
   Budget for comparison-group follow-up and a 3-month relationship check. Pool cohorts to
   reach adequate samples.

## Ready to go public? (per CLAUDE.md checklist)

| Step | 01 Atlas | 02 Mentorship | 03 Impact Engine |
|---|---|---|---|
| Rebuilds from scratch | Yes (verified identical) | Yes | Yes (deterministic seed) |
| Self-contained (copy `shared/fetch_data.py`, own requirements) | To do at move | To do at move | Yes (no downloads; benchmarks bundled) |
| No private/confidential data; small cells | Public aggregates only | Aggregates only | Synthetic only; suppression built in |
| Source licenses confirmed | Mostly: outcomes file is a Census public-use release; covariates file has no published license (link, don't re-host, or ask OI) | Mostly: Urban = ODC-By (attribution); Social Capital Atlas = Meta license; PISA: confirm OECD database terms | Yes: benchmarks inherit NSCH/YRBS (public domain) |
| Citations verified | Chetty et al. papers to confirm | Partly: DuBois 2011, Raposa 2019, Grossman & Rhodes 2002 checked; others to do | Partly: effect sizes checked (Raposa g = 0.21); Kiresuk & Sherman to confirm |
| Review by people who know the places/programs | Priority and beat-the-odds lists | Interpretation | Survey pilot with youth; comparison design with a partner |

### Round 2 readiness

| Step | 04 College Bridges | 05 Who's Around | 06 Adults in the Building | 07 Return on Mentoring |
|---|---|---|---|---|
| Rebuilds from scratch | Yes (Mobility Report Card file may need a manual download) | Yes | Yes | Yes (calculator checked against Python) |
| Licenses | Scorecard, Census: public domain; Social Capital Atlas: Meta license; Mobility Report Cards: no published license (link, don't re-host) | Public domain (BLS) | Public domain (ED) | Public domain (BLS); inherits 04 |
| Review | College-access staff review bridge list | None needed beyond verification | Verify ASCA 250:1 recommendation | Replace illustrative costs and effects with a real program's |

**08 Mentoring Evidence Engine:** rebuilds from ERIC bulk files (public domain, U.S. Department
of Education; the agent-coding stage is resumable but not cheap to rerun, so the committed
coded files are the record). Needs a human audit of a 50-record sample against full papers,
deduplication of multiple records per trial, and verification of every effect size before
external use.

**09 Federal Youth Program Investment Map:** rebuilds from keyless APIs (NSF, USAspending;
public domain) plus Census files; tags in `data/coded/` are the record. Needs a human
spot-check of 50 tags, and termination figures verified against NSF's published list (policy
sensitive: human review before any external use).

**10 Nonprofit Program DNA:** rebuilds from IRS bulk files (public domain; e-filed returns are
public records) plus Census files; tags in `data/coded/` are the record. Needs a human
spot-check, and community review of the candidate partner list before any outreach.

**11 AI and the Opportunity Ladder:** rebuilds from O*NET (CC BY 4.0: cite), Census summary
files, NCES and Scorecard (public domain), and Eloundou et al. labels (MIT, validation only);
ratings in `data/coded/` are the record. Needs a human spot-check of ratings and review of the
pathway lists with workforce partners.
