---
api_specs:
- filename: float16-openapi-generated.yml
  format: yaml
  label: Float16 API
  slug: float16-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/float16/refs/heads/main/openapi/_ae-authored/float16-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: float16.cloud
  spf: false
hosts:
- cert_expires: Apr 13 23:59:59 2027 GMT
  host: float16.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Float16 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Float16, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Float16
provider_slug: float16
slug: float16-domain-security
source_filename: float16-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: float16.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 13 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: float16.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/float16/refs/heads/main/security/float16-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloud
- API
- High-Performance Computing
- AI
---
