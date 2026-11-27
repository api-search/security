---
api_specs:
- filename: openmedici-com-v1-openapi.json
  format: json
  label: Open Medici Public API V1 API
  slug: open-medici-public-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmedici-com/openapi/_original/openmedici-com-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openmedici.com
  spf: true
hosts:
- cert_expires: Feb  7 12:47:25 2027 GMT
  host: openmedici.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Open Medici Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Medici, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Open Medici
provider_slug: openmedici-com
slug: openmedici-com-domain-security
source_filename: openmedici-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openmedici.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 12:47:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openmedici.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/openmedici-com/security/openmedici-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Grants
- Scholarships
- Research
- Fellowship
---
