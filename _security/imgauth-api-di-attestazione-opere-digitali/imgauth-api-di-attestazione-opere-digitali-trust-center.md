---
api_specs:
- filename: imgauth-api-di-attestazione-opere-digitali-openapi-original.json
  format: json
  label: imgauth REST API
  slug: imgauth-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imgauth-api-di-attestazione-opere-digitali/refs/heads/main/openapi/imgauth-api-di-attestazione-opere-digitali-openapi-original.json
certifications: []
description: ''
kind: trust-center
layout: security
name: Imgauth Api Di Attestazione Opere Digitali Trust Center
name_suffix: Trust Center
overview: imgauth — API di attestazione opere digitali maintains a public trust center covering its security and compliance posture.
provider_name: imgauth — API di attestazione opere digitali
provider_slug: imgauth-api-di-attestazione-opere-digitali
slug: imgauth-api-di-attestazione-opere-digitali-trust-center
source_filename: imgauth-api-di-attestazione-opere-digitali-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nprobe: true\nsource: https://trust.spaziogenesi.org/\nurl: https://trust.spaziogenesi.org/\ncertified: false\ncertifications: []\ncorrection: >-\n  The automated probe originally recorded SOC 2, ISO 27001 and GDPR here from keyword presence. Two of\n  those were WRONG and have been removed after reading the page. \"SOC 2\" and \"certificazione ISO 27001\"\n  appear on this page only inside a list of options the organisation EXAMINED AND DELIBERATELY REJECTED —\n  SOC 2 as irrelevant to an Italian public-interest audience, ISO 27001 certification as an unsustainable\n  audit cost for an ETS of this scale. The page states the Annex A controls are adopted \"per ispirazione,\n  non per certificazione formale\". Recording them as held certifications would have credited this\n  provider with a posture it explicitly disclaims.\nstandards_applied_without_certification:\n  - {id: 'ISO/IEC 27001', basis: 'Annex A controls relevant to the organisation''s\
  \ scale, applied for inspiration; no certification'}\n  - {id: 'ISO/IEC 27037', basis: partial — digital evidence acquisition and preservation}\n  - {id: 'ISO/IEC 27042', basis: partial — evidence analysis}\n  - {id: 'ISO/IEC 27043', basis: partial — incident investigation}\n  - {id: 'CAD + AgID guidelines', basis: digital document formation, PAdES B-LT with RFC 3161}\n  - {id: 'eIDAS 2.0', basis: 'explicitly NON-QUALIFIED positioning; qualified seal on the public roadmap, funding-dependent'}\nstandards_examined_and_rejected:\n  - {id: 'SOC 2', reason: 'US B2B enterprise standard, stated as having no relevance to the Italian public-interest audience'}\n  - {id: 'ISO 27001 certification', reason: 'audit cost disproportionate for an ETS of this scale'}\ncompliance_program:\n  published: true\n  name: Genesis Trust Framework (GTF)\n  components:\n    - Compliance Map — each standard with its applied/inspiration/rejected status\n    - Architecture Decision Records published in the repository\n\
  \    - Open Trust Score, computed from published formulas\n    - public risk register and annual review calendar\n    - technical whitepaper (CC BY 4.0)\n  note: >-\n    An open, self-published, auditable compliance program offered explicitly IN PLACE OF third-party\n    certification. It is genuine and unusually transparent for an organisation this size — but it is\n    self-attested, and any consumer should read it as such.\ngdpr:\n  implemented: true\n  evidence:\n    - data minimisation by design — file bytes never transit\n    - EU data residency (Cloudflare R2)\n    - cookieless Matomo analytics, no persistent identifiers\n    - published privacy notice and an admin \"forget\" flow that anonymises listings\ngovernance:\n  external_reviewer: Radixia srl (independent)\n  review_cadence: annual, published in the registry\n  human_cost_budget: 8 hours/month across all recurring processes\nsubprocessors:\n  - {name: Cloudflare, role: DNS, Workers, R2 storage, DDoS, Zero Trust Access}\n\
  \  - {name: GitHub, role: source, CI/CD, Pages}\n  - {name: Stripe, role: 'payments — hosted Checkout and Customer Portal, no card data on the Worker'}\n  - {name: Azure, role: digital signing service}\n  - {name: Telegram, role: optional attestation channel, user consent required}\n  - {name: OpenTimestamps calendar operators, role: Bitcoin anchor redundancy across 4 providers}\ndata_residency: EU\nevidence:\n  - source: https://trust.spaziogenesi.org/\n    http_status: 200\n    checked: '2026-08-11'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imgauth-api-di-attestazione-opere-digitali/refs/heads/main/security/imgauth-api-di-attestazione-opere-digitali-trust-center.yml
summary_line: trust center published
tags:
- digital notarization
- Timestamping
- proof-of-existence
- content authenticity
- Provenance
- Copyright
- IP protection
- Blockchain
- Bitcoin
- OpenTimestamps
- Security
- Document
- E-Signature
- MCP
trust_url: https://trust.spaziogenesi.org/
---
