---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: goodfellow.com
  spf: true
hosts:
- cert_expires: Sep 14 07:09:39 2026 GMT
  host: www.goodfellow.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Goodfellow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Goodfellow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Goodfellow
provider_slug: goodfellow
slug: goodfellow-domain-security
source_filename: goodfellow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goodfellow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 07:09:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: goodfellow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodfellow/refs/heads/main/security/goodfellow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advanced Materials
- Specialty Materials
- Metals
- Ceramics
- Polymers
- Composites
- Manufacturing
- Research
- Ecommerce
- Laboratory Services
---
