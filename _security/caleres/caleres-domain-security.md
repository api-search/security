---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: caleres.com
  spf: true
hosts:
- cert_expires: Aug 20 07:16:03 2026 GMT
  host: www.caleres.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caleres Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caleres, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Caleres
provider_slug: caleres
slug: caleres-domain-security
source_filename: caleres-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caleres.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 07:16:03 2026 GMT\n  hsts: null\ndomains:\n- domain: caleres.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caleres/refs/heads/main/security/caleres-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Footwear
- Retail
- Consumer Brands
- E-commerce
- Apparel
---
