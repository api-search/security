---
api_specs:
- filename: coolcollege-openapi-original.json
  format: json
  label: 酷学院 REST API (Cool College Open API)
  slug: 酷学院-rest-api-cool-college-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolcollege/refs/heads/main/openapi/coolcollege-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: coolcollege.cn
  spf: true
hosts:
- cert_expires: Sep 20 23:59:59 2026 GMT
  host: coolcollege.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Coolcollege Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 酷学院 (Cool College), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 酷学院 (Cool College)
provider_slug: coolcollege
slug: coolcollege-domain-security
source_filename: coolcollege-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coolcollege.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: coolcollege.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coolcollege/refs/heads/main/security/coolcollege-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Corporate Training
- E-Learning
- Talent Development
- Human Resources
- SaaS
- Learning Management
- China
---
