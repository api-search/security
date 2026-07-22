---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: crossoverhealth.com
  spf: true
hosts:
- cert_expires: Aug 28 08:27:27 2026 GMT
  host: crossoverhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crossoverhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crossoverhealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Crossoverhealth
provider_slug: crossoverhealth
slug: crossoverhealth-domain-security
source_filename: crossoverhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crossoverhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 08:27:27 2026 GMT\n  hsts: false\ndomains:\n- domain: crossoverhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crossoverhealth/refs/heads/main/security/crossoverhealth-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Primary Care
- Digital Health
- Telehealth
- Employer Health
- Care Navigation
- Occupational Medicine
---
