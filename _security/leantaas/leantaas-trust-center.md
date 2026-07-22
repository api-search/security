---
certifications:
- HITRUST CSF
- SOC 2
- HIPAA
description: LeanTaaS publishes a Vanta-hosted Trust Center at https://trust.leantaas.com/ covering its healthcare security and privacy posture. The page is a JavaScript-rendered single-page application whose control, document and subprocessor data is served from a signed-query GraphQL endpoint, so the automated trust-center probe recorded no keyword hit (the served HTML shell contains only metadata). The certifications below are NOT read from that shell — they are taken from Vanta's own published LeanTaaS customer story, which is a first-party statement by LeanTaaS's Director of Security & Compliance. Individual audit reports are gated behind the Trust Center's access/NDA flow and were not retrieved.
kind: trust-center
layout: security
name: Leantaas Trust Center
name_suffix: Trust Center
overview: LeanTaaS maintains a public trust center documenting HITRUST CSF, SOC 2, and HIPAA compliance.
provider_name: LeanTaaS
provider_slug: leantaas
slug: leantaas-trust-center
source_filename: leantaas-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: false\nurl: https://trust.leantaas.com/\nplatform: Vanta\nstatus: 200\ndescription: >-\n  LeanTaaS publishes a Vanta-hosted Trust Center at https://trust.leantaas.com/\n  covering its healthcare security and privacy posture. The page is a\n  JavaScript-rendered single-page application whose control, document and\n  subprocessor data is served from a signed-query GraphQL endpoint, so the\n  automated trust-center probe recorded no keyword hit (the served HTML shell\n  contains only metadata). The certifications below are NOT read from that\n  shell — they are taken from Vanta's own published LeanTaaS customer story,\n  which is a first-party statement by LeanTaaS's Director of Security &\n  Compliance. Individual audit reports are gated behind the Trust Center's\n  access/NDA flow and were not retrieved.\ncertifications:\n  - name: HITRUST CSF\n    version: r2\n    evidence: >-\n      \"In Vanta, LeanTaaS implemented HITRUST\
  \ r2 alongside HIPAA and SOC 2.\"\n      (vanta.com/customers/leantaas)\n  - name: SOC 2\n    evidence: >-\n      Named alongside HITRUST r2 and HIPAA as a framework LeanTaaS implemented\n      in Vanta (vanta.com/customers/leantaas). Report type (Type I vs Type II)\n      is not stated in the public source and is deliberately not asserted here.\n  - name: HIPAA\n    evidence: >-\n      Named alongside HITRUST r2 and SOC 2 (vanta.com/customers/leantaas).\n      LeanTaaS processes PHI on behalf of US hospitals and health systems.\nprograms:\n  - name: Vendor Risk Management\n    evidence: Listed in the Vanta customer story solution section.\n  - name: Questionnaire Automation\n    evidence: Listed in the Vanta customer story solution section.\n  - name: US state privacy laws\n    evidence: Listed in the Vanta customer story solution section.\ncontacts:\n  - role: Director of Security & Compliance\n    name: Bill Murphy\n    source: https://www.vanta.com/customers/leantaas\nreport_access:\
  \ >-\n  Audit reports and security documentation are requested through the Trust\n  Center access flow at https://trust.leantaas.com/ (Vanta gated documents).\n  No report was downloadable anonymously at probe time.\ndocs:\n  - https://trust.leantaas.com/\n  - https://trust.leantaas.com/resources\nevidence:\n  - source: https://trust.leantaas.com/\n    status: 200\n    observed: >-\n      Vanta trust-report SPA (slug 1tufob75d3j26ruz2igk1); certification names\n      not present in server-rendered HTML.\n  - source: https://www.vanta.com/customers/leantaas\n    status: 200\n    keywords: [hitrust r2, hipaa, soc 2]\nnotes: >-\n  No /.well-known/security.txt on leantaas.com (404) and no public bug bounty\n  or vulnerability-disclosure page was found, so no VulnerabilityDisclosure\n  artifact is emitted this round.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leantaas/refs/heads/main/security/leantaas-trust-center.yml
summary_line: HITRUST CSF, SOC 2, HIPAA
tags:
- Company
- Healthcare
- Health Systems
- Hospital Operations
- Capacity Management
- Artificial Intelligence
- Machine Learning
- Predictive Analytics
- Scheduling
- SaaS
trust_url: https://trust.leantaas.com/
---
