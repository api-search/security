---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: garmentory.com
  spf: true
hosts:
- cert_expires: Sep 20 23:59:59 2026 GMT
  host: garmentory.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Garmentory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Garmentory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Garmentory
provider_slug: garmentory
slug: garmentory-domain-security
source_filename: garmentory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: garmentory.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: garmentory.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/garmentory/refs/heads/main/security/garmentory-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Fashion
- Marketplace
- E-commerce
- Retail
- Apparel
- Boutiques
- Shopping
---
