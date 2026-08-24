---
certifications:
- SOC 1 Type II
- SOC 2 Type II
- ISO 27001
- ISO 9001
- FedRAMP Authorized
- StateRAMP Authorized
- CJIS
- CSA STAR Level 1
- CSA STAR Level 2
- Cyber Essentials
- CMMC 2.0
- FIPS 140-2
- HIPAA
- FERPA
- GDPR
description: ''
kind: trust-center
layout: security
name: Iboss Trust Center
name_suffix: Trust Center
overview: iboss maintains a public trust center documenting SOC 1 Type II, SOC 2 Type II, ISO 27001, ISO 9001, FedRAMP Authorized, StateRAMP Authorized, CJIS, CSA STAR Level 1, CSA STAR Level 2, Cyber Essentials, CMMC 2.0, FIPS 140-2, HIPAA, FERPA, and GDPR compliance.
provider_name: iboss
provider_slug: iboss
slug: iboss-trust-center
source_filename: iboss-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nsource: https://www.iboss.com/compliance\nnote: >-\n  iboss operates no dedicated trust-center subdomain (no trust.iboss.com), but it does\n  publish a real, substantive compliance and certifications page listing named, dated\n  attestations — which is the surface the trust_center check is looking for. The\n  automated probe (probe-security-programs.py) returned trust=none because it looks for\n  a trust-center host pattern; this artifact upgrades that to a searched result from the\n  page itself. Certifications are recorded AS PUBLISHED BY iboss. API Evangelist has not\n  audited or independently verified any of them.\ntrust_center:\n  present: true\n  url: https://www.iboss.com/compliance\n  status: 200\n  dedicated_subdomain: false\n  secondary_url: https://www.iboss.com/cloud-compliance-and-certifications\n  machine_readable: https://www.iboss.com/.well-known/brand-facts.json\n  note: >-\n    brand-facts.json carries a machine-readable\
  \ `certifications` array, which is unusual\n    and genuinely useful — most providers publish certifications only as page copy.\ncertifications:\n- {name: 'SOC 1 Type II', category: attestation, note: 'Non-CPA; internal controls over financial reporting'}\n- {name: 'SOC 2 Type II', category: attestation, note: 'Non-CPA; security, availability, confidentiality'}\n- {name: ISO 27001, category: certification, note: Information security management systems}\n- {name: ISO 9001, category: certification, note: Quality management systems}\n- {name: FedRAMP Authorized, category: government-authorization, note: US federal cloud services authorization}\n- {name: StateRAMP Authorized, category: government-authorization, note: US state and local government}\n- {name: CJIS, category: government-compliance, note: Criminal justice information handling}\n- {name: 'CSA STAR Level 1', category: cloud-assurance, note: Cloud Security Alliance self-assessment}\n- {name: 'CSA STAR Level 2', category: cloud-assurance,\
  \ note: Cloud Security Alliance third-party assessment}\n- {name: Cyber Essentials, category: certification, note: UK government-backed scheme}\n- {name: 'CMMC 2.0', category: readiness, note: '125 controls mapped across 14 security domains; published as readiness/coverage, not an award'}\n- {name: 'FIPS 140-2', category: validation, source: brand-facts.json}\n- {name: HIPAA, category: regulatory-alignment, source: brand-facts.json}\n- {name: FERPA, category: regulatory-alignment, source: brand-facts.json}\n- {name: GDPR, category: regulatory-alignment, source: brand-facts.json}\ndiscrepancy_note: >-\n  The /compliance page and /.well-known/brand-facts.json do not agree. The page lists\n  ISO 27001, ISO 9001, SOC 1 Type II, CSA STAR L1/L2 and Cyber Essentials, which\n  brand-facts.json omits; brand-facts.json lists FIPS 140-2, HIPAA, FERPA and GDPR,\n  which the page does not surface as badges. The union is recorded above with the\n  source of each. This is a real provider-side inconsistency\
  \ worth reporting back:\n  the machine-readable file iboss offers to AI engines is the LESS complete of the two.\nsub_processors:\n  published: false\npen_test_reports:\n  published: false\n  note: No public summary or on-request report portal was found.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iboss/refs/heads/main/security/iboss-trust-center.yml
summary_line: SOC 1 Type II, SOC 2 Type II, ISO 27001, ISO 9001, FedRAMP Authorized, StateRAMP Authorized, CJIS, CSA STAR Level 1, CSA STAR Level 2, Cyber Essentials, CMMC 2.0, FIPS 140-2, HIPAA, FERPA, GDPR
tags:
- Company
- Security
- Cybersecurity
- Zero Trust
- SASE
- Secure Web Gateway
- CASB
- ZTNA
- Data Loss Prevention
- Network Security
- Cloud Security
- Compliance
trust_url: ''
---
