---
api_specs:
- filename: buildonto-dev-batch-api-openapi.yml
  format: yaml
  label: Onto Batch API
  slug: buildonto-dev-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-batch-api-openapi.yml
- filename: buildonto-dev-extract-api-openapi.yml
  format: yaml
  label: Onto Extract API
  slug: buildonto-dev-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-extract-api-openapi.yml
- filename: buildonto-dev-map-api-openapi.yml
  format: yaml
  label: Onto Map API
  slug: buildonto-dev-map-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-map-api-openapi.yml
- filename: buildonto-dev-read-api-openapi.yml
  format: yaml
  label: Onto Read API
  slug: buildonto-dev-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-read-api-openapi.yml
- filename: buildonto-dev-read-score-api-openapi.yml
  format: yaml
  label: Onto Read + Score API
  slug: buildonto-dev-read-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-read-score-api-openapi.yml
- filename: buildonto-dev-score-api-openapi.yml
  format: yaml
  label: Onto Score API
  slug: buildonto-dev-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-score-api-openapi.yml
- filename: buildonto-dev-usage-api-openapi.yml
  format: yaml
  label: Onto Usage API
  slug: buildonto-dev-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: buildonto.dev
  spf: true
hosts:
- cert_expires: Jan 26 06:53:09 2027 GMT
  host: buildonto.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Onto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Onto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Onto
provider_slug: buildonto-dev
slug: buildonto-dev-domain-security
source_filename: buildonto-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buildonto.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 06:53:09 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: buildonto.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/buildonto-dev/security/buildonto-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Content
- Markdown
- Read API
- Platform
---
