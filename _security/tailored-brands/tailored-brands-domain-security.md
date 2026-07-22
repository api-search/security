---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tailoredbrands.com
  spf: true
hosts:
- cert_expires: Sep 17 21:51:18 2026 GMT
  host: www.tailoredbrands.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tailored Brands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tailored Brands, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tailored Brands
provider_slug: tailored-brands
slug: tailored-brands-domain-security
source_filename: tailored-brands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tailoredbrands.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 21:51:18 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: tailoredbrands.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tailored-brands/refs/heads/main/security/tailored-brands-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apparel
- E-Commerce
- Menswear
- Retail
---
