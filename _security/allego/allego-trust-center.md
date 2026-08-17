---
certifications:
- SOC 2 Type II
- ISO 27001
- GDPR
- UK Data Protection Law (UKDPL)
- CCPA
- FINRA 17a-3 / 17a-4
- FDA 21 CFR Part 11
- EU AI Act
description: Allego publishes a public trust portal at https://www.allego.com/trust/ covering security controls, AI data handling, availability, privacy compliance and regulated-industry standards. There is no gated trust-center vendor portal (Vanta/Drata/SafeBase) and no downloadable attestation; the certifications below are Allego's own published statements.
kind: trust-center
layout: security
name: Allego Trust Center
name_suffix: Trust Center
overview: Allego maintains a public trust center documenting SOC 2 Type II, ISO 27001, GDPR, UK Data Protection Law (UKDPL), CCPA, FINRA 17a-3 / 17a-4, FDA 21 CFR Part 11, and EU AI Act compliance.
provider_name: Allego
provider_slug: allego
slug: allego-trust-center
source_filename: allego-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "name: Allego Trust Portal\ndescription: >-\n  Allego publishes a public trust portal at https://www.allego.com/trust/ covering security\n  controls, AI data handling, availability, privacy compliance and regulated-industry\n  standards. There is no gated trust-center vendor portal (Vanta/Drata/SafeBase) and no\n  downloadable attestation; the certifications below are Allego's own published statements.\ngenerated: '2026-08-14'\nmethod: searched\nprobe: true\nsource: https://www.allego.com/trust/\nurl: https://www.allego.com/trust/\nhttp_status: 200\nfetched: '2026-08-14'\ncertifications:\n  - name: SOC 2 Type II\n    status: certified\n    detail: >-\n      \"SOC 2 Type II certified, with annual third-party penetration and vulnerability\n      testing.\"\n  - name: ISO 27001\n    status: aligned\n    detail: >-\n      \"Security practices align with ISO 27001 and OWASP standards, with code reviews\n      following Veracode standards.\" Allego's EU newsroom separately announces\
  \ achieving\n      ISO certifications. The trust portal wording is alignment, not certification.\n  - name: GDPR\n    status: compliant\n    detail: 'Complies with GDPR (EU 2016/679).'\n  - name: UK Data Protection Law (UKDPL)\n    status: compliant\n  - name: CCPA\n    status: compliant\n    detail: Plus \"applicable U.S. state privacy regulations\".\n  - name: FINRA 17a-3 / 17a-4\n    status: supported\n    detail: >-\n      \"Digital Safe supports FINRA 17a-3 and 17a-4 requirements for secure, immutable\n      records.\" Scoped to the Digital Safe capability.\n  - name: FDA 21 CFR Part 11\n    status: supported\n    detail: '\"Learning records support FDA 21 CFR Part 11 requirements.\"'\n  - name: EU AI Act\n    status: aligned\n    detail: '\"AI safeguards align with the EU AI Act and applicable regulatory standards.\"'\ncontrols:\n  encryption_in_transit: TLS 1.2\n  encryption_at_rest: minimum 256-bit\n  penetration_testing: annual third-party penetration and vulnerability testing\n\
  \  code_review: Veracode standards\n  physical: Data centers staffed 24x7 with strict physical access controls\n  access_control: >-\n    Role-based access controls; administrative responsibilities assignable by team or\n    region; approval workflows for external content sharing; each instance operates as a\n    separate security domain with no cross-instance access.\nai_data_handling:\n  training_on_customer_data: false\n  statements:\n    - Customer data is never used to train or fine-tune large language models.\n    - Data is used only to answer the request and is deleted immediately after the response is generated.\n    - Third-party AI providers do not retain, reuse, or learn from Allego customer data.\n    - Customer data is never shared across environments and never benefits another customer.\n    - All AI outputs are grounded in customer-approved content, with encryption in transit and at rest.\navailability:\n  infrastructure: Globally distributed, Amazon AWS and Microsoft Azure\n\
  \  storage: Amazon S3, designed for 99.999999999% durability over a given year\n  redundancy: Systems designed with redundancy to eliminate single points of failure\n  updates: Delivered without disrupting availability\n  status_page: https://status.allego.com/\n  sla_published: false\ndata_residency:\n  note: >-\n    \"Data processing, storage, and visibility controls align with GDPR and UK data\n    protection requirements.\" Works Council requirements are supported. Specific regional\n    hosting options are not enumerated publicly.\nvulnerability_disclosure:\n  published: false\n  security_txt: false\n  bug_bounty: false\n  note: >-\n    No security.txt on any Allego host, no published vulnerability disclosure policy and no\n    HackerOne/Bugcrowd/Intigriti program found. Allego states it performs annual third-party\n    penetration and vulnerability testing, but publishes no channel for external reporters.\n    No VulnerabilityDisclosure or Security pointer is emitted.\nevidence:\n\
  \  - source: https://www.allego.com/trust/\n    http_status: 200\n    keywords:\n      - soc 2 type ii\n      - iso 27001\n      - gdpr\n      - ccpa\n      - ukdpl\n      - finra 17a-4\n      - fda 21 cfr part 11\n      - eu ai act\n      - owasp\n      - veracode\n  - source: https://www.allego.com/.well-known/security.txt\n    http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allego/refs/heads/main/security/allego-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, GDPR, UK Data Protection Law (UKDPL), CCPA, FINRA 17a-3 / 17a-4, FDA 21 CFR Part 11, EU AI Act
tags:
- Sales Enablement
- Sales Training
- Video Coaching
- Content Management
- Conversation Intelligence
- Deal Intelligence
- Revenue Enablement
- Certifications
- AI
trust_url: https://www.allego.com/trust/
---
