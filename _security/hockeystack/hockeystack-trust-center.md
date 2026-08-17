---
certifications:
- SOC 2 Type 2
description: ''
kind: trust-center
layout: security
name: Hockeystack Trust Center
name_suffix: Trust Center
overview: HockeyStack maintains a public trust center documenting SOC 2 Type 2 compliance.
provider_name: HockeyStack
provider_slug: hockeystack
slug: hockeystack-trust-center
source_filename: hockeystack-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://security.hockeystack.com/\nplatform: Vanta Trust Center\nsummary: >-\n  HockeyStack runs a Vanta-powered Trust Center and states its certification in\n  plain text in its own product documentation. The prior round left certifications[]\n  empty because the Vanta SPA is not machine-extractable; this round sources the\n  certification from HockeyStack's own security documentation instead, which is a\n  first-party published statement.\ncertifications:\n- name: SOC 2 Type 2\n  status: certified\n  evidence: >-\n    \"HockeyStack has a SOC 2 Type 2 certification.\" — stated verbatim in the\n    provider's Security and Data Handling documentation.\n  source: https://agents-docs.hockeystack.com/sales-agents/security-and-data.md\n  verified: '2026-08-13'\n  artifacts_available: >-\n    Full documentation, including penetration test reports and certificates, is\n    offered via the Trust Center (gated request flow).\n\
  certifications_not_claimed:\n- ISO 27001\n- PCI DSS\n- HIPAA\n- FedRAMP\n- note: >-\n    None of these appear in the provider's security documentation. Absence recorded\n    deliberately — the Vanta SPA may display additional framework badges that could\n    not be read, so this is \"not claimed in readable docs\", not \"does not hold\".\nsecurity_program:\n  audits: internal and external audits\n  vulnerability_scanning:\n    tool: Qualys\n    cadence: continuous\n    retention: 6 months\n  security_monitoring:\n    tools:\n    - Datadog\n    - Sentry\n    log_retention: 1 year\n  penetration_testing: reports available via Trust Center\n  policy_reviews: annual review of data retention requirements\ndata_handling:\n  hosting:\n  - AWS\n  - MongoDB Atlas\n  data_residency: EU\n  on_premise: false\n  encryption_at_rest: true\n  encryption_in_transit: TLS 1.2 or higher\n  endpoint_controls:\n  - full disk encryption on employee devices\n  - 15-minute auto screen lock\n  - no removable media\n\
  \  access_control: >-\n    Confidential classification; role-restricted need-to-know access; documented\n    data-owner approval required for non-preapproved roles; no anonymous or\n    unauthenticated access to systems storing customer data; customer data never\n    used in non-production environments.\n  retention: lifetime of contract\n  deletion_after_termination: within 30 days\n  early_deletion: on verified request, confirmed in writing\n  subprocessor_sharing: >-\n    Limited to service delivery (AWS, MongoDB Atlas); transfers require written\n    management approval and a governing contract; vendors assessed under a\n    Third-Party Management Policy.\nai_data_commitments:\n  customer_data_used_for_training: false\n  scope: >-\n    Applies to HockeyStack and to all AI sub-processors powering Sales Agents.\n    Inputs and outputs sent to model providers are not retained for training.\n  contractual: true\n  contract_location: DPA\n  note: >-\n    A contractual no-training commitment\
  \ extended to sub-processors is materially\n    stronger than the policy-page assurance most vendors in this category publish.\n  source: https://agents-docs.hockeystack.com/sales-agents/security-and-data.md\nincident_response:\n  documented: true\n  customer_notification: per contractual commitments and applicable law\n  forensic_retention: 1 year\ntrust_center_probe:\n  url: https://security.hockeystack.com/\n  http_status: 200\n  machine_readable: false\n  detail: >-\n    Vanta trust-report app; /api/trust-report also returns the SPA shell rather than\n    JSON, and api.vanta.com returns 401 without credentials. Framework badges are\n    rendered client-side and remain unextractable, which is why the certification\n    above is sourced from the docs instead.\n  checked: '2026-08-13'\nevidence:\n- source: https://agents-docs.hockeystack.com/sales-agents/security-and-data.md\n  status: 200\n  provides: SOC 2 Type 2 claim, data residency, retention, AI training commitments\n- source: https://security.hockeystack.com/\n\
  \  status: 200\n  provides: Trust Center existence and canonical URL\nnotes: >-\n  A `Compliance` pointer is now wired in apis.yml on the strength of the named,\n  first-party SOC 2 Type 2 statement. No `Security` (vulnerability disclosure)\n  pointer is wired — see security/ for that probe; HockeyStack publishes no\n  security.txt, no bug bounty and no disclosure policy.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hockeystack/refs/heads/main/security/hockeystack-trust-center.yml
summary_line: SOC 2 Type 2
tags:
- Company
- Data
- Marketing Analytics
- Attribution
- Revenue Intelligence
- B2B
- Account Intelligence
- MCP
- AI Agents
trust_url: https://security.hockeystack.com/
---
