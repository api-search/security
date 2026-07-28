---
certifications:
- SOC 2 Type 2
- SOC 2 Type 1
- PCI DSS
description: ''
kind: trust-center
layout: security
name: Flo Ev Trust Center
name_suffix: Trust Center
overview: FLO maintains a public trust center documenting SOC 2 Type 2, SOC 2 Type 1, and PCI DSS compliance.
provider_name: FLO
provider_slug: flo-ev
slug: flo-ev-trust-center
source_filename: flo-ev-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nprobe: true\nurl: https://trust.flo.com/\ntitle: FLO Trust Center\nplatform: Vanta\nplatform_evidence: >-\n  trust.flo.com is a CNAME to 67eec921f6325d6c3432909a.cname.vantatrust.com; the\n  page is served from assets.vanta.com with canonical https://trust.flo.com and\n  <title>FLO Trust Center</title>. HTTP 200, TLS 1.3, HSTS max-age=31536000;\n  includeSubDomains.\ncontent_access: >-\n  The trust center renders client-side from a signed Vanta GraphQL API\n  (POST /graphql returns \"Missing `signature` or `signedAt`\"), so the\n  certification and subprocessor lists are not readable anonymously via HTTP.\n  The certification below is therefore evidenced from FLO's own press release\n  rather than scraped from the trust center shell.\ncertifications:\n- name: SOC 2 Type 2\n  auditor: BARR Advisory\n  announced: '2024-10-22'\n  source: https://www.flo.com/news/flo-achieves-major-cybersecurity-soc-2-type-2-certification/\n  quote: >-\n\
  \    FLO states the SOC 2 Type 2 audit \"covers a wide range of security controls\n    and supports operational effectiveness over time\", was performed by \"BARR\n    Advisory, a leading provider of cloud-based security and compliance\n    solutions\", and that FLO will recertify annually.\n- name: SOC 2 Type 1\n  auditor: BARR Advisory\n  announced: '2024'\n  status: superseded by SOC 2 Type 2\n  source: https://www.flo.com/en-ca/press-release/flo-affirms-commitment-to-network-and-data-security-with-soc-2-type-1-certification/\n- name: PCI DSS\n  status: claimed-in-marketing\n  note: >-\n    FLO states its network-connected stations include a PCI-DSS compliant\n    payment system. This is a product statement on FLO's own pages, not an\n    attestation document, and no AOC or certificate number is published.\nnot_found:\n  iso_27001: not published\n  fedramp: not applicable / not published\n  hipaa: not applicable\n  csa_star: not published\n  subprocessor_list: not readable anonymously\n\
  evidence:\n- {source: 'https://trust.flo.com/', status: 200, kind: trust center, keywords: [trust center, security, compliance]}\n- {source: 'https://www.flo.com/news/flo-achieves-major-cybersecurity-soc-2-type-2-certification/', kind: press release, certification: SOC 2 Type 2}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flo-ev/refs/heads/main/security/flo-ev-trust-center.yml
summary_line: SOC 2 Type 2, SOC 2 Type 1, PCI DSS
tags:
- Energy
- Canada
- EV Charging
- Electricity
- Grid
- Demand Response
- Interoperability
- OCPP
- OCPI
- OpenADR
- Charge Point Operator
- Quebec
trust_url: https://trust.flo.com/
---
