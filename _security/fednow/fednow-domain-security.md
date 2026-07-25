---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: frbservices.org
  spf: true
hosts:
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: www.frbservices.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fednow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FedNow Service, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FedNow Service
provider_slug: fednow
slug: fednow-domain-security
source_filename: fednow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.frbservices.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: frbservices.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fednow/refs/heads/main/security/fednow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- United States
- Real-Time Payments
- Instant Payments
- ISO 20022
- Account-to-Account
- Scheme Operator
- Federal Reserve
---
