---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hookerfurniture.com
  spf: true
hosts:
- cert_expires: Oct  6 21:08:09 2026 GMT
  host: www.hookerfurniture.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- host: developer.hookerfurniture.com
  https: false
- host: api.hookerfurniture.com
  https: false
kind: domain-security
layout: security
method: probed
name: Hooker Furniture Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hooker Furniture, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hooker Furniture
provider_slug: hooker-furniture
slug: hooker-furniture-domain-security
source_filename: hooker-furniture-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hookerfurniture.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:08:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developer.hookerfurniture.com\n  https: false\n- host: api.hookerfurniture.com\n  https: false\ndomains:\n- domain: hookerfurniture.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hooker-furniture/refs/heads/main/security/hooker-furniture-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Furniture
- Home Products
---
