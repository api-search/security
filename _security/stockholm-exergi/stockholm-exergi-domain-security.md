---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stockholmexergi.se
  spf: true
hosts:
- cert_expires: Apr  3 09:21:34 2027 GMT
  host: stockholmexergi.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stockholm Exergi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stockholm Exergi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stockholm Exergi
provider_slug: stockholm-exergi
slug: stockholm-exergi-domain-security
source_filename: stockholm-exergi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stockholmexergi.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  3 09:21:34 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stockholmexergi.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stockholm-exergi/refs/heads/main/security/stockholm-exergi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- DistrictHeating
- Sustainability
- Sweden
---
