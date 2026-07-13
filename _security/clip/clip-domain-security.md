---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clip.mx
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: payclip.com
  spf: true
hosts:
- cert_expires: Sep 16 05:45:02 2026 GMT
  host: www.clip.mx
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 17:24:53 2026 GMT
  host: www.payclip.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 07:15:40 2026 GMT
  host: developer.clip.mx
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clip, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clip
provider_slug: clip
slug: clip-domain-security
source_filename: clip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clip.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 05:45:02 2026 GMT\n  hsts: false\n- host: www.payclip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 17:24:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.clip.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 07:15:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clip.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: payclip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clip/refs/heads/main/security/clip-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Acquiring
- SMB Payments
- Point of Sale
- mPOS
- Tap to Pay
- Card Acceptance
- Checkout
- Payment Gateway
- Payment Links
- Mexico
- Latin America
- Fintech
- PCI
---
