---
api_specs:
- filename: encore-framework-openapi.yml
  format: yaml
  label: Encore Framework API
  slug: encore-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encore-dev/refs/heads/main/openapi/encore-framework-openapi.yml
- filename: encore-platform-openapi.yml
  format: yaml
  label: Encore Cloud Platform API
  slug: encore-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encore-dev/refs/heads/main/openapi/encore-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: encore.cloud
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: encore.dev
  spf: true
hosts:
- cert_expires: Sep  3 01:54:37 2026 GMT
  host: encore.cloud
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 22:32:38 2026 GMT
  host: encore.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 16:53:53 2026 GMT
  host: api.encore.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Encore Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Encore, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Encore
provider_slug: encore-dev
slug: encore-dev-domain-security
source_filename: encore-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: encore.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 01:54:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: encore.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 22:32:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.encore.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:53:53 2026 GMT\n  hsts: null\ndomains:\n- domain: encore.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: encore.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/encore-dev/refs/heads/main/security/encore-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Backend
- Framework
- Cloud
- TypeScript
- Go
- DeveloperTools
- InfrastructureFromCode
- Microservices
- Observability
- Multicloud
---
