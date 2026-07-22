---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: avis-budget.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: avisbudgetgroup.com
  spf: true
hosts:
- cert_expires: Oct  7 01:46:39 2026 GMT
  host: www.avis-budget.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.avisbudgetgroup.com
  https: false
kind: domain-security
layout: security
method: probed
name: Avis Budget Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avis Budget, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Avis Budget
provider_slug: avis-budget
slug: avis-budget-domain-security
source_filename: avis-budget-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avis-budget.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 01:46:39 2026 GMT\n  hsts: false\n- host: developer.avisbudgetgroup.com\n  https: false\ndomains:\n- domain: avis-budget.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: avisbudgetgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avis-budget/refs/heads/main/security/avis-budget-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fortune 500
- Car Rental
- Travel
- Mobility
- Fleet Management
- Transportation
---
