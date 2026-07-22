---
api_specs:
- filename: revyze-openapi.json
  format: json
  label: Revyze API
  slug: revyze-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revyze/refs/heads/main/openapi/revyze-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: revyze.fr
  spf: true
hosts:
- cert_expires: Oct  5 15:08:39 2026 GMT
  host: www.revyze.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: api.revyze.fr
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Revyze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revyze, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Revyze
provider_slug: revyze
slug: revyze-domain-security
source_filename: revyze-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.revyze.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 15:08:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.revyze.fr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: revyze.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revyze/refs/heads/main/security/revyze-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- EdTech
- Education
- Mobile
- Video
- Learning
- Quiz
- France
- GraphQL
---
