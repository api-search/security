---
api_specs:
- filename: university-of-adelaide-figshare.yaml
  format: yaml
  label: Adelaide Figshare Research Data API
  slug: figshare
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-figshare.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adelaide.edu.au
  spf: true
- caa:
  - 0 issue "harica.gr"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: figshare.com
  spf: true
hosts:
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: www.adelaide.edu.au
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: digital.library.adelaide.edu.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: adelaide.figshare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Adelaide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Adelaide, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Adelaide
provider_slug: university-of-adelaide
slug: university-of-adelaide-domain-security
source_filename: university-of-adelaide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adelaide.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: digital.library.adelaide.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: false\n- host: adelaide.figshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: adelaide.edu.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: figshare.com\n  dnssec: false\n  caa:\n  - 0 issue \"harica.gr\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/security/university-of-adelaide-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Institutional Repository
- Open Data
- Australia
---
