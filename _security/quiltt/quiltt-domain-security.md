---
api_specs:
- filename: quiltt-openapi.yml
  format: yaml
  label: Quiltt Profiles API
  slug: quiltt-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quiltt/refs/heads/main/openapi/quiltt-openapi.yml
- filename: quiltt-openapi.yml
  format: yaml
  label: Quiltt Connections API
  slug: quiltt-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quiltt/refs/heads/main/openapi/quiltt-openapi.yml
- filename: quiltt-openapi.yml
  format: yaml
  label: Quiltt Session Tokens API
  slug: quiltt-session-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quiltt/refs/heads/main/openapi/quiltt-openapi.yml
- filename: quiltt-openapi.yml
  format: yaml
  label: Quiltt Webhooks API
  slug: quiltt-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quiltt/refs/heads/main/openapi/quiltt-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: quiltt.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: quiltt.dev
  spf: true
hosts:
- cert_expires: Sep  5 12:46:43 2026 GMT
  host: www.quiltt.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 22:20:56 2026 GMT
  host: www.quiltt.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 16:22:53 2026 GMT
  host: api.quiltt.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quiltt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quiltt, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Quiltt
provider_slug: quiltt
slug: quiltt-domain-security
source_filename: quiltt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quiltt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 12:46:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.quiltt.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 22:20:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.quiltt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 16:22:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: quiltt.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: quiltt.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quiltt/refs/heads/main/security/quiltt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fintech
- Open Banking
- Financial Data
- Aggregation
- GraphQL
---
