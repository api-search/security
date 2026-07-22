---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: c16bio.com
  spf: true
hosts:
- cert_expires: Sep 19 19:29:44 2026 GMT
  host: www.c16bio.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: C16 Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for C16 Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: C16 Biosciences
provider_slug: c16-biosciences
slug: c16-biosciences-domain-security
source_filename: c16-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.c16bio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 19:29:44 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: c16bio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/c16-biosciences/refs/heads/main/security/c16-biosciences-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Synthetic Biology
- Biotechnology
- Sustainable Ingredients
- Palm Oil Alternative
- Consumer Goods
- Fermentation
- Climate Tech
---
