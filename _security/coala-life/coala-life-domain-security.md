---
api_specs:
- filename: coala-life-patientsessions-api-openapi.yml
  format: yaml
  label: Coala Life Patient Sessions API
  slug: coala-life-patientsessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coala-life/refs/heads/main/openapi/coala-life-patientsessions-api-openapi.yml
- filename: coala-life-platform-api-api-openapi.yml
  format: yaml
  label: Coala Life Platform.Api API
  slug: coala-life-platform-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coala-life/refs/heads/main/openapi/coala-life-platform-api-api-openapi.yml
- filename: coala-life-sessions-api-openapi.yml
  format: yaml
  label: Coala Life Sessions API
  slug: coala-life-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coala-life/refs/heads/main/openapi/coala-life-sessions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: coalalife.com
  spf: true
hosts:
- cert_expires: Nov 22 19:45:32 2026 GMT
  host: www.coalalife.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coala Life Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coala Life, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Coala Life
provider_slug: coala-life
slug: coala-life-domain-security
source_filename: coala-life-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coalalife.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 19:45:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: coalalife.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coala-life/refs/heads/main/security/coala-life-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Cardiology
- Remote Monitoring
- Digital Health
---
