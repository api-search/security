---
api_specs:
- filename: dp-bohrium-openapi.json
  format: json
  label: Bohrium OpenAPI
  slug: bohrium-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dp/refs/heads/main/openapi/dp-bohrium-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dp.tech
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bohrium.com
  spf: true
hosts:
- cert_expires: Nov 29 09:23:25 2026 GMT
  host: dp.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: open.bohrium.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DP Technology (Bohrium), probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DP Technology (Bohrium)
provider_slug: dp
slug: dp-domain-security
source_filename: dp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dp.tech\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 29 09:23:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: open.bohrium.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: dp.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: bohrium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dp/refs/heads/main/security/dp-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- AI for Science
- Scientific Computing
- Molecular Simulation
- Drug Discovery
- Materials Science
- Research Cloud
- Machine Learning
- HPC
---
