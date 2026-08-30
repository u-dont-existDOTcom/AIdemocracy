# Architecture baselines: Taiwan + United States

Date: 2026-08-30
Status: active design input for Observable UN / AI Democracy
Disposition: **compose**, not invent

## Independent conception preserved before this scan

The project starts from a public cognitive/audit layer around democratic and multilateral institutions rather than a sovereign AI: make mandates, money, implementation, evidence, outcomes and disagreements legible; use AI to retrieve, compare, audit and mediate; preserve provenance and dissent; keep political/coercive authority with humans.

## Taiwan baseline — participatory process

Taiwan is the strongest practical baseline located so far for the democratic-participation side.

Mechanisms to reuse or adapt:

1. **Consensus discovery rather than engagement-ranking.** vTaiwan uses Polis to cluster participants by response patterns and surface statements that bridge groups rather than rewarding replies, virality or outrage.
2. **No-reply interaction where useful.** Participants agree/disagree/pass on statements rather than building adversarial reply trees. This reduces trolling and makes opinion geometry legible.
3. **Online + offline sandwich.** Digital large-scale listening is embedded in a facilitated process with agenda setting, stakeholder preparation, collaborative meetings and policy follow-through.
4. **Institutional Participation Officers.** Agencies designate empowered staff who translate between public language and policy machinery, coordinate cross-agency issues, facilitate deliberation and publish the process.
5. **Radical process transparency.** Collaborative meetings publish transcripts/video and retain traceable process records. Diversity of views is treated as more important than raw headcount.
6. **Participation across the policy lifecycle.** Taiwan's JOIN platform separates proposal, discussion, supervision and direct contact rather than treating democracy as one election or comment box.
7. **Government response obligation.** Citizen proposals that pass a threshold require a responsible-agency response under the JOIN process.
8. **Open source / inspectability as political infrastructure.** Formal political deliberation should not depend on an opaque engagement-ranking system.

Primary references:
- https://info.vtaiwan.tw/
- https://join.gov.tw/aboutus/index/en_US
- https://po.pdis.nat.gov.tw/en/meeting-process/
- https://theme.ndc.gov.tw/lawout/EngLawContent.aspx?id=57&lan=E
- https://pdis.nat.gov.tw/en/blog/%E5%A0%85%E5%BC%B7%E6%B0%91%E4%B8%BB-%E6%95%B8%E4%BD%8D%E6%B0%91%E5%9C%8B/
- https://compdemocracy.org/polis/book/introduction/

## United States baseline — public observability substrate

The U.S. federal government has many of the machine-readable pieces needed for an Observable Government system, but they are fragmented.

Reusable components:

- **Federal Program Inventory (FPI):** program identities and some funding/performance information. GAO reported in March 2026 that the inventory covered more than 2,600 programs and over $7T in FY2024 expenditures but still failed to meet 13 of 20 statutory requirements and omitted important program/performance information.
- **USAspending.gov:** public API for awards, accounts, transactions, recipients, agencies and spending.
- **SAM.gov:** procurement opportunities and award-related federal acquisition infrastructure.
- **Oversight.gov:** cross-Inspector-General reports and searchable open recommendations.
- **GAO:** open recommendations, duplication/fragmentation work, program-performance audits and quantified potential benefits.
- **Performance.gov:** agency strategic and priority-goal reporting.
- **Regulations.gov / Federal Register:** public rulemaking dockets, comments and supporting documents.
- **EPA public-comment AI:** EPA states that for some rulemakings it may use AI to sort/categorize comments, identify substantive comments, separate arguments by topic/theme and generate individual summaries, with required human supervision and human-drafted responses.

Primary references:
- https://fpi.omb.gov/
- https://www.gao.gov/products/gao-26-107551
- https://api.usaspending.gov/
- https://sam.gov/opportunities
- https://www.oversight.gov/reports/recommendations
- https://www.performance.gov/about/faq/
- https://www.regulations.gov/
- https://www.epa.gov/dockets/commenting-epa-dockets

## What neither baseline currently provides

No located deployment integrates all of the following as one public system:

law/mandate → program → budget → award/procurement → implementer → action → performance/outcomes → audit findings/recommendations → public/stakeholder positions → institutional response

with source-level provenance, explicit missing links, cross-source contradiction detection, disagreement decomposition and public consensus mapping.

The architectural direction is therefore:

**Taiwan's participatory process + U.S. public-data/audit substrate + standards-based provenance + UN/multilateral institutional layer.**

## Design consequences for the demonstrator

- The dashboard must not be a conventional KPI dashboard. It must expose the causal/authority chain and missing links.
- A future deliberation surface should prioritize cross-group consensus and disagreement geometry, not likes or comment volume.
- Public comments/preferences must not automatically become votes; evidence quality, affected-party status, representativeness and normative preference are distinct signals.
- Human review and contestability remain mandatory for AI-generated clustering, summaries, classifications and inferred relationships.
- Every material synthesized claim must be expandable to its source records.
- The system should support explicit dissent and competing model interpretations rather than one official AI truth layer.
