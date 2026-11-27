---
api_specs:
- filename: lazaretto-dev-attestations-api-openapi.yml
  format: yaml
  label: Lazaretto Attestations API
  slug: lazaretto-dev-attestations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-attestations-api-openapi.yml
- filename: lazaretto-dev-benchmark-json-api-openapi.yml
  format: yaml
  label: Lazaretto Benchmark.json API
  slug: lazaretto-dev-benchmark-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-benchmark-json-api-openapi.yml
- filename: lazaretto-dev-check-api-openapi.yml
  format: yaml
  label: Lazaretto Check API
  slug: lazaretto-dev-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-check-api-openapi.yml
- filename: lazaretto-dev-checkout-api-openapi.yml
  format: yaml
  label: Lazaretto Checkout API
  slug: lazaretto-dev-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-checkout-api-openapi.yml
- filename: lazaretto-dev-credits-api-openapi.yml
  format: yaml
  label: Lazaretto Credits API
  slug: lazaretto-dev-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-credits-api-openapi.yml
- filename: lazaretto-dev-health-api-openapi.yml
  format: yaml
  label: Lazaretto Health API
  slug: lazaretto-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-health-api-openapi.yml
- filename: lazaretto-dev-known-bad-api-openapi.yml
  format: yaml
  label: Lazaretto Known Bad API
  slug: lazaretto-dev-known-bad-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-known-bad-api-openapi.yml
- filename: lazaretto-dev-lockfile-api-openapi.yml
  format: yaml
  label: Lazaretto Lockfile API
  slug: lazaretto-dev-lockfile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-lockfile-api-openapi.yml
- filename: lazaretto-dev-mcp-api-openapi.yml
  format: yaml
  label: Lazaretto MCP API
  slug: lazaretto-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-mcp-api-openapi.yml
- filename: lazaretto-dev-rules-api-openapi.yml
  format: yaml
  label: Lazaretto Rules API
  slug: lazaretto-dev-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-rules-api-openapi.yml
- filename: lazaretto-dev-scan-api-openapi.yml
  format: yaml
  label: Lazaretto Scan API
  slug: lazaretto-dev-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-scan-api-openapi.yml
- filename: lazaretto-dev-trial-api-openapi.yml
  format: yaml
  label: Lazaretto Trial API
  slug: lazaretto-dev-trial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-trial-api-openapi.yml
- filename: lazaretto-dev-usage-api-openapi.yml
  format: yaml
  label: Lazaretto Usage API
  slug: lazaretto-dev-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-usage-api-openapi.yml
- filename: lazaretto-dev-verify-api-openapi.yml
  format: yaml
  label: Lazaretto Verify API
  slug: lazaretto-dev-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-verify-api-openapi.yml
- filename: lazaretto-dev-watch-api-openapi.yml
  format: yaml
  label: Lazaretto Watch API
  slug: lazaretto-dev-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-watch-api-openapi.yml
- filename: lazaretto-dev-well-known-api-openapi.yml
  format: yaml
  label: Lazaretto .well Known API
  slug: lazaretto-dev-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazaretto-dev/openapi/lazaretto-dev-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lazaretto.dev
  spf: true
hosts:
- cert_expires: Feb  6 11:47:27 2027 GMT
  host: lazaretto.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lazaretto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lazaretto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Lazaretto
provider_slug: lazaretto-dev
slug: lazaretto-dev-domain-security
source_filename: lazaretto-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lazaretto.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 11:47:27 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lazaretto.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lazaretto-dev/security/lazaretto-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- npm
- Malware
- Open Source
---
