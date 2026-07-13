---
api_specs:
- filename: cityu-scholars-pure-ws.yaml
  format: yaml
  label: CityUHK Scholars Pure Web Service (REST)
  slug: scholars-pure-ws
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cityu/refs/heads/main/openapi/cityu-scholars-pure-ws.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cityu.edu.hk
  spf: true
hosts:
- cert_expires: Sep 28 12:36:15 2026 GMT
  host: www.cityu.edu.hk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: scholars.cityu.edu.hk
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cityu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for City University of Hong Kong, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: City University of Hong Kong
provider_slug: cityu
slug: cityu-domain-security
source_filename: cityu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cityu.edu.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:36:15 2026 GMT\n  hsts: false\n- host: scholars.cityu.edu.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: cityu.edu.hk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cityu/refs/heads/main/security/cityu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Institutional Repository
- OAI-PMH
- Hong Kong
- China
---
