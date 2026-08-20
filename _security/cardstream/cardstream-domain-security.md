---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cardstream.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gitbook.io
  spf: true
hosts:
- cert_expires: Oct 12 11:51:26 2026 GMT
  host: cardstream.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 19:03:12 2026 GMT
  host: guides.gitbook.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 11:51:26 2026 GMT
  host: gateway.cardstream.com
  hsts: true
  hsts_max_age: 660
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cardstream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cardstream, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cardstream
provider_slug: cardstream
slug: cardstream-domain-security
source_filename: cardstream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cardstream.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 11:51:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: guides.gitbook.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 19:03:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway.cardstream.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 11:51:26 2026 GMT\n  hsts: true\n  hsts_max_age: 660\ndomains:\n- domain: cardstream.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: gitbook.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardstream/refs/heads/main/security/cardstream-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- United Kingdom
- Payment Gateway
- Payment Processing
- White Label
- Card Payments
- Acquiring
- Hosted Payment Pages
- Tokenization
- 3D Secure
- Alternative Payment Methods
- Subscription
---
