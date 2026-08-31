---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tailorbrands.com
  spf: true
hosts:
- cert_expires: Oct 12 03:25:22 2026 GMT
  host: www.tailorbrands.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 03:25:22 2026 GMT
  host: api.tailorbrands.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tailor Brands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tailor Brands, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tailor Brands
provider_slug: tailor-brands
slug: tailor-brands-domain-security
source_filename: tailor-brands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tailorbrands.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:25:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tailorbrands.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:25:22 2026 GMT\n  hsts: null\ndomains:\n- domain: tailorbrands.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tailor-brands/refs/heads/main/security/tailor-brands-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Business Formation
- Compliance
- Small Business
- Branding
- Legal
- Registered Agent
- Embedded Finance
- Artificial Intelligence
- Logo Design
---
