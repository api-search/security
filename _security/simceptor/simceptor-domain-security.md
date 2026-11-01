---
api_specs:
- filename: simceptor-openapi-generated.yml
  format: yaml
  label: Simceptor API
  slug: simceptor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simceptor/openapi/_ae-authored/simceptor-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: simceptor.com
  spf: true
hosts:
- cert_expires: Dec 27 00:15:22 2026 GMT
  host: simceptor.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Simceptor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simceptor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Simceptor
provider_slug: simceptor
slug: simceptor-domain-security
source_filename: simceptor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simceptor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 00:15:22 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: simceptor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/simceptor/security/simceptor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mock API
- No-Code
- AI Integration
- Developer Tools
---
