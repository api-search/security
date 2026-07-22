---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brooksbrothers.com
  spf: true
hosts:
- cert_expires: Aug  6 16:50:48 2026 GMT
  host: www.brooksbrothers.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brooks Brothers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brooks Brothers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Brooks Brothers
provider_slug: brooks-brothers
slug: brooks-brothers-domain-security
source_filename: brooks-brothers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brooksbrothers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  6 16:50:48 2026 GMT\n  hsts: null\ndomains:\n- domain: brooksbrothers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brooks-brothers/refs/heads/main/security/brooks-brothers-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Retail
- Fashion
- Apparel
- Menswear
- Luxury Clothing
---
