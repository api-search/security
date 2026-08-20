---
certifications:
- SOC 2 Type 2
description: ''
kind: trust-center
layout: security
name: Intricately Trust Center
name_suffix: Trust Center
overview: Intricately maintains a public trust center documenting SOC 2 Type 2 compliance.
provider_name: Intricately
provider_slug: intricately
slug: intricately-trust-center
source_filename: intricately-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://trust.hginsights.com/\nscope: parent-organization\napi: Cloud Dynamics API (Intricately)\nnote: >-\n  READ THIS BEFORE USING THIS FILE AS EVIDENCE. Intricately publishes no trust\n  center, no security page and no certification claim on any of its own hosts —\n  kb.intricately.com, help.intricately.com and status.intricately.com carry none,\n  and /.well-known/security.txt is 404 everywhere (see\n  well-known/intricately-well-known.yml). The trust center recorded here belongs to\n  HG Insights, the parent that acquired Intricately in March 2022 and to whose site\n  intricately.com now 301-redirects. It is the governing corporate entity for the\n  API, and its Terms of Service page carries a \"Cloud Dynamics\" login item pointing\n  at https://my.intricately.com/ — but the trust center itself never names\n  Intricately or Cloud Dynamics, and asserts nothing about this API's controls.\n  For that reason apis.yml wires\
  \ `TrustCenter` and does NOT wire `Compliance`: the\n  compliance program is real, and it is the parent's, and no published document\n  extends it to this product.\ntrust_center:\n  url: https://trust.hginsights.com/\n  operator: HG Insights, Inc.\n  relationship_to_provider: acquirer / parent brand\n  acquired: '2022-03-29'\n  http_status: 200\n  access: >-\n    Landing page is public; the underlying reports and policies are request-gated\n    behind the trust-center access flow.\n  names_this_product: false\ncertifications:\n- name: SOC 2 Type 2\n  status: listed\n  document_access: request-gated\n  scope_covers_intricately: unstated\nreports_offered:\n- SOC 2 Report\n- Pentest Report\n- Network Diagram\nself_assessments:\n- CAIQ\n- SIG Lite\npolicy_documents_listed:\n- Acceptable Use Policy\n- Asset Management Policy\n- Backup Policy\n- Business Continuity / Disaster Recovery Policy\n- Data Classification Policy\n- Data Protection Policy\n- Data Retention Policy\ncontrol_domains_listed:\n\
  - Data Security\n- Access Control\n- Infrastructure\n- Endpoint Security\n- Corporate Security\n- Asset Management\n- BC/DR\n- Training\n- Physical & Environmental\nintricately_surfaces_checked:\n- url: https://help.intricately.com/\n  status: 200\n  finding: no security or compliance collection\n- url: https://kb.intricately.com/llms.txt\n  status: 200\n  finding: 31 documentation pages indexed, none about security or compliance\n- url: https://api.intricately.com/.well-known/security.txt\n  status: 404\n  finding: no security.txt\n- url: https://intricately.com/\n  status: 200\n  finding: 301 redirect chain terminating at https://hginsights.com/\nvulnerability_disclosure:\n  published: false\n  note: >-\n    No security.txt, no bug bounty program (HackerOne / Bugcrowd / Intigriti all\n    negative), and no coordinated-disclosure page on any Intricately or HG Insights\n    surface found. No VulnerabilityDisclosure artifact is written and no `Security`\n    pointer is emitted.\nchecked:\
  \ '2026-08-14'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intricately/refs/heads/main/security/intricately-trust-center.yml
summary_line: SOC 2 Type 2
tags:
- Company
- Sales Intelligence
- Cloud Intelligence
- Technographics
- Data Enrichment
- Cloud Spend
- Market Intelligence
trust_url: ''
---
