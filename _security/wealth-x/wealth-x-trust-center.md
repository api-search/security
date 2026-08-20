---
api_specs:
- filename: wealth-x-dossiers-api-openapi.yml
  format: yaml
  label: Wealth-X Dossiers API
  slug: wealth-x-dossiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealth-x/refs/heads/main/openapi/wealth-x-dossiers-api-openapi.yml
- filename: wealth-x-reference-api-openapi.yml
  format: yaml
  label: Wealth-X Reference API
  slug: wealth-x-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealth-x/refs/heads/main/openapi/wealth-x-reference-api-openapi.yml
- filename: wealth-x-search-api-openapi.yml
  format: yaml
  label: Wealth-X Search API
  slug: wealth-x-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealth-x/refs/heads/main/openapi/wealth-x-search-api-openapi.yml
certifications:
- SOC 2
- CCPA Validation
description: Wealth-X publishes no security or trust page of its own, and probe-security-programs.py found no security.txt, bug bounty, or trust center on any wealthx.com host. Its parent Altrata publishes a named compliance posture on "Altrata's Privacy Promise", and the llms.txt served from Wealth-X's own domain (https://wealthx.com/llms.txt) states plainly that "Altrata is a subsidiary of Delinian and is SOC 2 certified."
kind: trust-center
layout: security
name: Wealth X Trust Center
name_suffix: Trust Center
overview: Wealth-X maintains a public trust center documenting SOC 2 and CCPA Validation compliance.
provider_name: Wealth-X
provider_slug: wealth-x
slug: wealth-x-trust-center
source_filename: wealth-x-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://altrata.com/altratas-privacy-promise\ndescription: >-\n  Wealth-X publishes no security or trust page of its own, and\n  probe-security-programs.py found no security.txt, bug bounty, or trust center\n  on any wealthx.com host. Its parent Altrata publishes a named compliance\n  posture on \"Altrata's Privacy Promise\", and the llms.txt served from\n  Wealth-X's own domain (https://wealthx.com/llms.txt) states plainly that\n  \"Altrata is a subsidiary of Delinian and is SOC 2 certified.\"\ntrust_center_url: https://altrata.com/altratas-privacy-promise\npublic_portal: false\nportal_note: >-\n  There is no self-serve trust portal (no Vanta/Drata/SafeBase instance;\n  trust.altrata.com does not resolve). Audit reports are gated: \"we ... make our\n  audit reports – along with our full collection of security documentation –\n  available to clients and prospects upon request.\"\ncertifications:\n  - name: SOC 2\n    type:\
  \ attestation\n    status: claimed\n    verified_by_us: false\n    evidence: >-\n      \"We regularly invest in independent auditors to assess our security\n      environment as part of our SOC2 attestation.\" and \"On an annual basis, an\n      independent expert third party auditor assesses our security environment\n      in detail as part of our commitments to maintain our SOC2 attestation.\n      Please contact a member of our commercial team for a copy of our SOC-2\n      report.\"\n    source: https://altrata.com/altratas-privacy-promise\n    report_access: on request via the Altrata commercial team\n  - name: CCPA Validation\n    type: independent validation\n    status: achieved\n    verified_by_us: false\n    evidence: >-\n      \"Altrata has achieved independent CCPA Validation confirming that our\n      privacy practices meet established CCPA Controls. Following a detailed\n      assessment and evidence review...\" A downloadable \"Altrata Inc. CCPA\n      Validation Findings\
  \ Letter\" is published on the page.\n    source: https://altrata.com/altratas-privacy-promise\nregulatory_compliance:\n  - regime: GDPR\n    posture: >-\n      Data controller relying on legitimate interests as its Article 6(1) lawful\n      basis, with documented Legitimate Interest Assessments and Standard\n      Contractual Clauses where applicable.\n    source: https://altrata.com/altratas-privacy-promise\n  - regime: CCPA / CPRA\n    posture: >-\n      Compliant, with a published \"Do Not Sell\" rights process and independent\n      CCPA Validation.\n    source: https://altrata.com/altratas-privacy-promise\n  - regime: China PIPL\n    posture: Named as a standard Altrata states it is compliant with.\n    source: https://altrata.com/altratas-privacy-promise\n  - regime: US state data broker registration\n    posture: >-\n      Altrata holds current data broker registrations in California, Oregon,\n      Texas and Vermont — material for a provider whose product is third-party\n   \
  \   personal data on private individuals.\n    source: https://altrata.com/altratas-privacy-promise\nsecurity_practices:\n  - practice: Independent annual third-party security assessment\n    source: https://altrata.com/altratas-privacy-promise\n  - practice: Continuous penetration testing\n    source: https://altrata.com/altratas-privacy-promise\n  - practice: Patch and vulnerability management process\n    source: https://altrata.com/altratas-privacy-promise\n  - practice: Documented data deletion policy\n    source: https://altrata.com/altratas-privacy-promise\n  - practice: Security-by-design process and personnel security training\n    source: https://altrata.com/altratas-privacy-promise\ngaps:\n  - No published security.txt on wealthx.com, connect.wealthx.com or altrata.com (all 404).\n  - No vulnerability disclosure policy or bug bounty program found.\n  - No self-serve trust portal; every artifact is gated behind a sales conversation.\n  - No compliance page on wealthx.com itself\
  \ — the entire posture is published under the parent brand.\nevidence:\n  - url: https://altrata.com/altratas-privacy-promise\n    status: 200\n  - url: https://wealthx.com/llms.txt\n    status: 200\n    note: '\"Altrata is a subsidiary of Delinian and is SOC 2 certified.\" — served from Wealth-X''s own domain.'\n  - url: https://altrata.com/.well-known/security.txt\n    status: 404\n  - url: https://wealthx.com/.well-known/security.txt\n    status: 404\n  - url: https://trust.altrata.com/\n    status: 0\n    note: Host does not resolve.\n  - url: https://altrata.com/compliance\n    status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wealth-x/refs/heads/main/security/wealth-x-trust-center.yml
summary_line: SOC 2, CCPA Validation
tags:
- Company
- Wealth Intelligence
- Data
- UHNW
- Prospecting
- Financial-Services
- CRM
- People Data
- Altrata
- GraphQL
- MCP
- Wealth Screening
trust_url: ''
---
