---
api_specs:
- filename: university-of-canterbury-figshare-api.yaml
  format: yaml
  label: Canterbury Figshare (figshare REST and OAI-PMH)
  slug: figshare-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-canterbury/refs/heads/main/openapi/university-of-canterbury-figshare-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: canterbury.ac.nz
  spf: true
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "certainly.com"
  - 0 issue "harica.gr"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: figshare.com
  spf: true
hosts:
- cert_expires: Aug 25 20:43:18 2026 GMT
  host: www.canterbury.ac.nz
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 05:30:34 2026 GMT
  host: ir.canterbury.ac.nz
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: canterbury.figshare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Canterbury Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Canterbury, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of Canterbury
provider_slug: university-of-canterbury
slug: university-of-canterbury-domain-security
source_filename: university-of-canterbury-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.canterbury.ac.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 20:43:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: ir.canterbury.ac.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 05:30:34 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: canterbury.figshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: canterbury.ac.nz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: figshare.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"harica.gr\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-canterbury/refs/heads/main/security/university-of-canterbury-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Repository
- OAI-PMH
- New Zealand
---
