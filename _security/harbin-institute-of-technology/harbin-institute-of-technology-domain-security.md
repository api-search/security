---
api_specs:
- filename: harbin-institute-of-technology-pure.yaml
  format: yaml
  label: HIT Research Portal OAI-PMH
  slug: pure-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbin-institute-of-technology/refs/heads/main/openapi/harbin-institute-of-technology-pure.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hit.edu.cn
  spf: true
hosts:
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: en.hit.edu.cn
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: scholar.hit.edu.cn
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Harbin Institute Of Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harbin Institute of Technology, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Harbin Institute of Technology
provider_slug: harbin-institute-of-technology
slug: harbin-institute-of-technology-domain-security
source_filename: harbin-institute-of-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.hit.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\n- host: scholar.hit.edu.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hit.edu.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harbin-institute-of-technology/refs/heads/main/security/harbin-institute-of-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Education
- Higher Education
- University
- Research
- Scholarly
- OAI-PMH
- China
---
