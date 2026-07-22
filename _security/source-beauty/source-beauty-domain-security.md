---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sourcebeauty.com
  spf: false
hosts:
- cert_expires: Sep  8 16:31:03 2026 GMT
  host: sourcebeauty.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Source Beauty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Source Beauty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Source Beauty
provider_slug: source-beauty
slug: source-beauty-domain-security
source_filename: source-beauty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sourcebeauty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 16:31:03 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: sourcebeauty.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/source-beauty/refs/heads/main/security/source-beauty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Beauty
- Cosmetics
- E-commerce
- Retail
- Marketplace
- Wellness
- Egypt
- Skincare
- Consumer
---
