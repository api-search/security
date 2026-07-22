---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ofx.com
  spf: true
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: www.ofx.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 23:59:59 2026 GMT
  host: developer.ofx.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: api.ofx.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ozforex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OFX (OzForex), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OFX (OzForex)
provider_slug: ozforex
slug: ozforex-domain-security
source_filename: ozforex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ofx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developer.ofx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  4 23:59:59 2026 GMT\n  hsts: null\n- host: api.ofx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ofx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ozforex/refs/heads/main/security/ozforex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Money Transfer
- Foreign Exchange
- International Payments
- Payments
- Currency
- Fintech
---
