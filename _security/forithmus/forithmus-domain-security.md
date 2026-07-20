---
api_specs:
- filename: forithmus-openapi-original.json
  format: json
  label: Forithmus Challenge Platform API
  slug: forithmus-challenge-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forithmus/refs/heads/main/openapi/forithmus-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forithmus.com
  spf: true
hosts:
- cert_expires: Oct 10 07:47:07 2026 GMT
  host: forithmus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Forithmus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forithmus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Forithmus
provider_slug: forithmus
slug: forithmus-domain-security
source_filename: forithmus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forithmus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 07:47:07 2026 GMT\n  hsts: false\ndomains:\n- domain: forithmus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forithmus/refs/heads/main/security/forithmus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Medical Imaging
- Radiology
- Machine Learning
- Foundation Models
- Healthcare AI
- Challenge Platform
- Benchmarks
- Research
- Developer Tools
- API
---
