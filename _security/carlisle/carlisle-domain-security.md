---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: carlisle.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: customersuccesslogin.com
  spf: true
hosts:
- cert_expires: Aug 26 01:57:27 2026 GMT
  host: www.carlisle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: customersuccesslogin.com
  https: false
kind: domain-security
layout: security
method: probed
name: Carlisle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carlisle Companies, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Carlisle Companies
provider_slug: carlisle
slug: carlisle-domain-security
source_filename: carlisle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carlisle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 01:57:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: customersuccesslogin.com\n  https: false\ndomains:\n- domain: carlisle.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: customersuccesslogin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carlisle/refs/heads/main/security/carlisle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Building Envelope
- Building Products
- Construction
- Contractor Portal
- Distributors
- EDI
- Insulation
- Manufacturing
- Roofing
- Waterproofing
- Fortune 1000
---
