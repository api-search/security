---
api_specs:
- filename: toneperfect-assessment-api-openapi.yml
  format: yaml
  label: TonePerfect (Pronunciation Assessment API) Assessment API
  slug: toneperfect-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toneperfect/refs/heads/main/openapi/toneperfect-assessment-api-openapi.yml
- filename: toneperfect-capabilities-api-openapi.yml
  format: yaml
  label: TonePerfect (Pronunciation Assessment API) Capabilities API
  slug: toneperfect-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toneperfect/refs/heads/main/openapi/toneperfect-capabilities-api-openapi.yml
- filename: toneperfect-utilities-api-openapi.yml
  format: yaml
  label: TonePerfect (Pronunciation Assessment API) Utilities API
  slug: toneperfect-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toneperfect/refs/heads/main/openapi/toneperfect-utilities-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: toneperfect.app
  spf: false
hosts:
- cert_expires: Dec 26 06:34:31 2026 GMT
  host: api.toneperfect.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Toneperfect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TonePerfect (Pronunciation Assessment API), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: TonePerfect (Pronunciation Assessment API)
provider_slug: toneperfect
slug: toneperfect-domain-security
source_filename: toneperfect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.toneperfect.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 06:34:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: toneperfect.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toneperfect/refs/heads/main/security/toneperfect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Speech
- Language-Learning
- Pronunciation
---
