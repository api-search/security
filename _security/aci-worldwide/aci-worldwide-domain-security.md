---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: aciworldwide.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: oppwa.com
  spf: true
hosts:
- cert_expires: Oct 16 19:43:24 2026 GMT
  host: www.aciworldwide.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 11:00:29 2026 GMT
  host: docs.aciworldwide.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 00:48:45 2026 GMT
  host: eu-prod.oppwa.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aci Worldwide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ACI Worldwide, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ACI Worldwide
provider_slug: aci-worldwide
slug: aci-worldwide-domain-security
source_filename: aci-worldwide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aciworldwide.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 19:43:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.aciworldwide.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 11:00:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eu-prod.oppwa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 00:48:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aciworldwide.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: oppwa.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aci-worldwide/refs/heads/main/security/aci-worldwide-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- United States
- Payment Gateway
- Payment Processing
- Acquiring
- Card Payments
- eCommerce
- Fraud
- Tokenization
- 3D Secure
- Bill Payment
- Real-Time Payments
- ISO 20022
---
