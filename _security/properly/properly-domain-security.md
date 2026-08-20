---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: properly.ca
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pine.ca
  spf: true
hosts:
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: properly.ca
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 03:01:57 2026 GMT
  host: www.pine.ca
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Properly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Properly, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Properly
provider_slug: properly
slug: properly-domain-security
source_filename: properly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: properly.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.pine.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 03:01:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: properly.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: pine.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/properly/refs/heads/main/security/properly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- Canada
- Property Listings
- MLS
- Valuation
- AVM
- PropTech
- Mortgage
---
