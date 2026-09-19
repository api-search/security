---
certification_count: 2
certifications:
- SOC 2 Type II
- ISO/IEC 27001:2022
description: 'Trust center and published compliance program covering G2 Track, operated by BetterCloud. The trust center itself is a Vanta-hosted client-rendered page: the served HTML is a 5.4KB SPA shell, so the certification list below was read from BetterCloud''s own first-party security-and-compliance page rather than scraped from the trust center.'
kind: trust-center
layout: security
name: G2 Track Trust Center
name_suffix: Trust Center
overview: G2 Track maintains a public trust center documenting SOC 2 Type II and ISO/IEC 27001:2022 compliance.
provider_name: G2 Track
provider_slug: g2-track
slug: g2-track-trust-center
source_filename: g2-track-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: https://trust.bettercloud.com/ + https://www.bettercloud.com/security-and-compliance/\nprovider: G2 Track\nproviderId: g2-track\ndescription: >-\n  Trust center and published compliance program covering G2 Track, operated by BetterCloud. The\n  trust center itself is a Vanta-hosted client-rendered page: the served HTML is a 5.4KB SPA shell,\n  so the certification list below was read from BetterCloud's own first-party security-and-compliance\n  page rather than scraped from the trust center.\ntrust_center:\n  url: https://trust.bettercloud.com/\n  platform: Vanta\n  status: 200\n  probed: '2026-09-12'\n  machine_readable: false\n  note: >-\n    JS-rendered. /api/trust-report and /api/v1/trust-center both return the same SPA shell, so no\n    structured certification feed is reachable anonymously.\ncertifications:\n- name: SOC 2 Type II\n  status: attested\n  scope: security, availability, processing integrity, confidentiality,\
  \ privacy\n  evidence: https://www.bettercloud.com/security-and-compliance/\n  report_access: on request via Customer Success Manager or Account Executive\n- name: ISO/IEC 27001:2022\n  status: certified\n  evidence: https://www.bettercloud.com/security-and-compliance/\n  note: BetterCloud publishes the certificate for download from its own site.\nprivacy_regimes:\n- name: GDPR\n  mechanism: Data Processing Addendum + Main Subscription Agreement\n  evidence: https://www.bettercloud.com/security-and-compliance/\n- name: CCPA\n  mechanism: Main Subscription Agreement + Data Processing Addendum\n  evidence: https://www.bettercloud.com/security-and-compliance/\n- name: UK Data Protection Act 2018 / UK GDPR\n  mechanism: Data Processing Addendum\n  evidence: https://www.bettercloud.com/security-and-compliance/\nnot_claimed:\n- HIPAA\n- FedRAMP\n- PCI DSS\n- StateRAMP\n- TX-RAMP\nnot_claimed_note: >-\n  Recorded as an honest absence: none of these appear on BetterCloud's security-and-compliance\
  \ page.\n  Absence here is not a finding against the provider, only a statement of what is published.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/g2-track/refs/heads/main/security/g2-track-trust-center.yml
summary_line: SOC 2 Type II, ISO/IEC 27001:2022
tags:
- Contract Management
- SaaS Management
- Spend Optimization
- Shadow IT
- License Management
- Software Asset Management
- IT Operations
trust_url: ''
---
