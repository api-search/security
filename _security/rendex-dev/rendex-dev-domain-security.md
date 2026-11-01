---
api_specs:
- filename: rendex-dev-account-api-openapi.yml
  format: yaml
  label: rendex-dev Account API
  slug: rendex-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendex-dev/openapi/rendex-dev-account-api-openapi.yml
- filename: rendex-dev-batch-api-openapi.yml
  format: yaml
  label: rendex-dev Batch API
  slug: rendex-dev-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendex-dev/openapi/rendex-dev-batch-api-openapi.yml
- filename: rendex-dev-health-api-openapi.yml
  format: yaml
  label: rendex-dev Health API
  slug: rendex-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendex-dev/openapi/rendex-dev-health-api-openapi.yml
- filename: rendex-dev-jobs-api-openapi.yml
  format: yaml
  label: rendex-dev Jobs API
  slug: rendex-dev-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendex-dev/openapi/rendex-dev-jobs-api-openapi.yml
- filename: rendex-dev-screenshot-api-openapi.yml
  format: yaml
  label: rendex-dev Screenshot API
  slug: rendex-dev-screenshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendex-dev/openapi/rendex-dev-screenshot-api-openapi.yml
- filename: rendex-dev-watch-api-openapi.yml
  format: yaml
  label: rendex-dev Watch API
  slug: rendex-dev-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendex-dev/openapi/rendex-dev-watch-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rendex.dev
  spf: true
hosts:
- cert_expires: Dec 25 22:09:30 2026 GMT
  host: rendex.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rendex Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for rendex-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: rendex-dev
provider_slug: rendex-dev
slug: rendex-dev-domain-security
source_filename: rendex-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rendex.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 22:09:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rendex.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/rendex-dev/security/rendex-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Rendering
- Screenshot
- PDF
- API
- Automation
---
