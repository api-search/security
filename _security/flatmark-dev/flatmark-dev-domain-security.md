---
api_specs:
- filename: flatmark-dev-account-api-openapi.yml
  format: yaml
  label: flatmark Account API
  slug: flatmark-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flatmark-dev/openapi/flatmark-dev-account-api-openapi.yml
- filename: flatmark-dev-convert-api-openapi.yml
  format: yaml
  label: flatmark Convert API
  slug: flatmark-dev-convert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flatmark-dev/openapi/flatmark-dev-convert-api-openapi.yml
- filename: flatmark-dev-jobs-api-openapi.yml
  format: yaml
  label: flatmark Jobs API
  slug: flatmark-dev-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flatmark-dev/openapi/flatmark-dev-jobs-api-openapi.yml
- filename: flatmark-dev-webhooks-api-openapi.yml
  format: yaml
  label: flatmark Webhooks API
  slug: flatmark-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flatmark-dev/openapi/flatmark-dev-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flatmark.dev
  spf: true
hosts:
- cert_expires: Jan 29 05:32:01 2027 GMT
  host: flatmark.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: flatmark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for flatmark, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: flatmark
provider_slug: flatmark-dev
slug: flatmark-dev-domain-security
source_filename: flatmark-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flatmark.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 05:32:01 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flatmark.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/flatmark-dev/security/flatmark-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- PDF
- Markdown
- Conversion
- RAG
---
