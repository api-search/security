---
api_specs:
- filename: amazingtalker-find-tutors-openapi.yml
  format: yaml
  label: AmazingTalker Find Tutors
  slug: amazingtalker-find-tutors
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazingtalker/refs/heads/main/openapi/amazingtalker-find-tutors-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: amazingtalker.com
  spf: false
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: en.amazingtalker.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazingtalker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AmazingTalker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AmazingTalker
provider_slug: amazingtalker
slug: amazingtalker-domain-security
source_filename: amazingtalker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.amazingtalker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: amazingtalker.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazingtalker/refs/heads/main/security/amazingtalker-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Education
- Tutoring
- Language Learning
- Marketplace
- EdTech
- ChatGPT Plugin
---
