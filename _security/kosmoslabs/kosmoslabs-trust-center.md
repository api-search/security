---
certifications: []
description: 'Kosmos AI Labs, Inc operates a public Security Trust Center at trust.kosmoslabs.ai. IMPORTANT — it publishes a compliance PROGRAM, not achieved certifications: both SOC 2 Type 1 and SOC 2 Type 2 are listed "In progress" and zero certifications are complete. An earlier automated probe of this page recorded "SOC 2, ISO 27001" from the trust-center vendor''s boilerplate meta description ("...against common cybersecurity frameworks like SOC 2, ISO 27001, ISO 9001, and more"); that was a false positive and has been corrected. Kosmos does not claim ISO 27001 anywhere.'
kind: trust-center
layout: security
name: Kosmoslabs Trust Center
name_suffix: Trust Center
overview: Kosmos AI Labs maintains a public trust center covering its security and compliance posture.
provider_name: Kosmos AI Labs
provider_slug: kosmoslabs
slug: kosmoslabs-trust-center
source_filename: kosmoslabs-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nsource: https://trust.kosmoslabs.ai/ and https://kosmoslabs.ai/resources/security/\nurl: https://trust.kosmoslabs.ai/\ndescription: >-\n  Kosmos AI Labs, Inc operates a public Security Trust Center at trust.kosmoslabs.ai. IMPORTANT —\n  it publishes a compliance PROGRAM, not achieved certifications: both SOC 2 Type 1 and SOC 2\n  Type 2 are listed \"In progress\" and zero certifications are complete. An earlier automated probe\n  of this page recorded \"SOC 2, ISO 27001\" from the trust-center vendor's boilerplate meta\n  description (\"...against common cybersecurity frameworks like SOC 2, ISO 27001, ISO 9001, and\n  more\"); that was a false positive and has been corrected. Kosmos does not claim ISO 27001\n  anywhere.\n\ntrust_center:\n  published: true\n  url: https://trust.kosmoslabs.ai/\n  title: Kosmos AI Labs, Inc - Security Trust Center\n  status: 200\n  probed: '2026-07-19'\n  secondary_page: https://kosmoslabs.ai/resources/security/\n\
  \ncertifications_achieved: []\n\ncertifications_in_progress:\n- name: SOC 2 Type 1\n  status: in progress\n  target: >-\n    \"SOC 2 Type 1 targeted Audit engaged · Jun 2026\" (security page); trust center FAQ states\n    completion targeted for June 2026.\n  evidence: Listed as \"In progress\" on trust.kosmoslabs.ai; audit engagement published.\n- name: SOC 2 Type 2\n  status: in progress\n  evidence: Listed as \"In progress\" on trust.kosmoslabs.ai.\n\niso_27001:\n  claimed: false\n  note: >-\n    Not claimed on the trust center or the security page. Present only in the trust-center\n    vendor's generic meta-description boilerplate.\n\nprogram_metrics:\n  source: https://trust.kosmoslabs.ai/\n  frameworks_tracked: 2\n  controls_monitored: 35\n  controls_note: Continuously monitored across infrastructure and processes.\n  internal_policies: 25\n  subprocessors_listed: 0\n  documents_available: 0\n\npenetration_testing:\n  conducted: true\n  detail: >-\n    \"Penetration testing is part\
  \ of our SOC 2 preparation program. Results are available to\n    customers\" (trust center FAQ).\n  public_report: false\n\nsecurity_testing:\n  dast:\n    published: true\n    result: 0 findings High severity\n    date: Mar 2026\n    source: https://kosmoslabs.ai/resources/security/\n\ndpa:\n  available: true\n  note: DPA requests routed to the security alias; trust center FAQ confirms a DPA is available.\n\nquestionnaires:\n  supported: [VSA, CAIQ, custom questionnaires]\n  sla: Five business days\n  routing: Dedicated security alias (security@kosmoslabs.ai)\n  source: https://kosmoslabs.ai/resources/security/\n\nsecurity_posture:\n  encryption_in_transit: TLS 1.2+\n  integration_scopes: OAuth 2.0 with read-only integration scopes by default\n  trust_model: '\"Machines propose. Humans confirm.\"'\n  source: https://docs.kosmoslabs.ai/product-documentation/security-overview\n\nrelated:\n  domain_security: security/kosmoslabs-domain-security.yml\n  vulnerability_disclosure: security/kosmoslabs-vulnerability-disclosure.yml\n\
  \  conformance: conformance/kosmoslabs-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kosmoslabs/refs/heads/main/security/kosmoslabs-trust-center.yml
summary_line: trust center published
tags:
- Company
- Operational Intelligence
- Observability
- OpenTelemetry
- Incident Management
- Root Cause Analysis
- AIOps
- Enterprise Software
trust_url: https://trust.kosmoslabs.ai/
---
