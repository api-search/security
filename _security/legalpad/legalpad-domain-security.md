---
description: ''
domains:
- caa: []
  created: '2018-01-09'
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: legalpad.io
  mx: true
  mx_provider: Google Workspace
  nameservers:
  - ns-368.awsdns-46.com
  - ns-704.awsdns-24.net
  - ns-1289.awsdns-33.org
  - ns-1808.awsdns-34.co.uk
  registered: true
  registrar: Gandi SAS
  spf: false
  updated: '2025-12-10'
hosts:
- dns_a: []
  evidence: NXDOMAIN/no-A on apex
  host: legalpad.io
  https: false
  resolves: false
- dns_a: []
  host: www.legalpad.io
  https: false
  resolves: false
- dns_a: []
  host: beta.legalpad.io
  https: false
  note: sign-in host linked from the archived homepage
  resolves: false
- dns_a: []
  host: get.legalpad.io
  https: false
  note: events/webinars host linked from the archived homepage
  resolves: false
- dns_a: []
  host: api.legalpad.io
  https: false
  note: probed speculatively; never documented by the provider
  resolves: false
- dns_a: []
  host: app.legalpad.io
  https: false
  note: probed speculatively; never documented by the provider
  resolves: false
kind: domain-security
layout: security
method: probed
name: Legalpad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LegalPad, probed live across 6 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LegalPad
provider_slug: legalpad
slug: legalpad-domain-security
source_filename: legalpad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: dig + curl against legalpad.io and its known subdomains\nnote: >-\n  Legalpad was acquired by Deel in 2022 and its web presence was retired after 2024. The\n  legalpad.io domain is still registered (Gandi, renewed 2025-12-10) and still routes email\n  via Google Workspace MX, but publishes no A/AAAA records on the apex or on any subdomain\n  observed in the archived site, so there is no live HTTPS host to probe. Absence of records\n  is recorded as observed data, not as a failure.\nhosts:\n- host: legalpad.io\n  dns_a: []\n  resolves: false\n  https: false\n  evidence: NXDOMAIN/no-A on apex\n- host: www.legalpad.io\n  dns_a: []\n  resolves: false\n  https: false\n- host: beta.legalpad.io\n  dns_a: []\n  resolves: false\n  https: false\n  note: sign-in host linked from the archived homepage\n- host: get.legalpad.io\n  dns_a: []\n  resolves: false\n  https: false\n  note: events/webinars host linked from the archived homepage\n\
  - host: api.legalpad.io\n  dns_a: []\n  resolves: false\n  https: false\n  note: probed speculatively; never documented by the provider\n- host: app.legalpad.io\n  dns_a: []\n  resolves: false\n  https: false\n  note: probed speculatively; never documented by the provider\ndomains:\n- domain: legalpad.io\n  registered: true\n  registrar: Gandi SAS\n  created: '2018-01-09'\n  updated: '2025-12-10'\n  nameservers:\n  - ns-368.awsdns-46.com\n  - ns-704.awsdns-24.net\n  - ns-1289.awsdns-33.org\n  - ns-1808.awsdns-34.co.uk\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n  mx: true\n  mx_provider: Google Workspace\nsuccessor_domain:\n  domain: deel.com\n  note: >-\n    Live posture for the successor service belongs to the Deel provider record\n    (all/deel/), not to this archived company profile.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/legalpad/refs/heads/main/security/legalpad-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Legal
- Immigration
- Work Visas
- Legal Services
- Human Resources
- Employment
- Global Mobility
- Professional Services
---
