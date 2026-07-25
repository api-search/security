---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: myzeller.com
  spf: true
hosts:
- cert_expires: Oct  7 09:01:33 2026 GMT
  host: www.myzeller.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zeller Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zeller, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zeller
provider_slug: zeller
slug: zeller-domain-security
source_filename: zeller-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.myzeller.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 09:01:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: myzeller.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeller/refs/heads/main/security/zeller-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Australia
- Payment Gateway
- Payment Processing
- Acquiring
- Merchant Services
- Point of Sale
- In-Person Payments
- Tap to Pay
- SME
---
