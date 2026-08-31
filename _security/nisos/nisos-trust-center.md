---
certifications: []
description: ''
kind: trust-center
layout: security
name: Nisos Trust Center
name_suffix: Trust Center
overview: Nisos maintains a public trust center covering its security and compliance posture.
provider_name: Nisos
provider_slug: nisos
slug: nisos-trust-center
source_filename: nisos-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://trust.nisos.com/\nurl: https://trust.nisos.com/\nplatform: Vanta\ncertifications: []\nevidence:\n  - url: https://trust.nisos.com/\n    status: 200\n    content_type: text/html\n    note: >-\n      Live, first-party trust center on a Nisos-controlled subdomain, hosted by Vanta —\n      the served HTML carries data-signature-manifest-url pointing at assets.vanta.com,\n      a canonical link to https://trust.nisos.com, and the title \"Nisos Trust Center\".\n  - url: https://trust.nisos.com/.well-known/zzz-control-probe-9182\n    status: 200\n    note: >-\n      Control probe returned the identical 5,433-byte body, confirming the host is a\n      single-page app that answers 200 for every path.\nreadability: js-rendered\nnote: >-\n  The trust center is real and reachable, but its content — the certification list, the\n  document library and the subprocessor register — is rendered client-side from the Vanta\n  API. The served\
  \ HTML contains no framework name, so NO certification (SOC 2, ISO 27001,\n  HIPAA, FedRAMP, PCI DSS) could be verified anonymously and none is asserted here. The\n  automated probe (0-working/probe-security-programs.py) correctly declined to write on the\n  same evidence; this file records the page's existence without inventing its contents.\npointer_policy: >-\n  A TrustCenter pointer is emitted in apis.yml against the live page. NO Compliance pointer\n  is emitted — compliance_published requires a named, published certification, and naming\n  one we could not read would be fabrication.\nvulnerability_disclosure:\n  found: false\n  probed:\n    - url: https://nisos.com/.well-known/security.txt\n      status: 404\n    - url: https://ascend.nisos.com/.well-known/security.txt\n      status: 200\n      note: SPA catch-all, not a security.txt — see well-known/nisos-well-known.yml\n  note: >-\n    No security.txt, no /security or /vulnerability-disclosure page in the 144-URL page\n    sitemap,\
  \ and no HackerOne, Bugcrowd or Intigriti program found. No Security pointer is\n    emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nisos/refs/heads/main/security/nisos-trust-center.yml
summary_line: trust center published
tags:
- Threat Intelligence
- Human Risk Management
- Insider Threat
- Executive Protection
- OSINT
- Digital Investigations
- Cybersecurity
- Adversary Attribution
- Employment Fraud
- Third-Party Risk
- Trust and Safety
- Dark Web Monitoring
- Managed Service
- Federal
trust_url: https://trust.nisos.com/
---
