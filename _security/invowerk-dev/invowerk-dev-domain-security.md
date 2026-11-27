---
api_specs:
- filename: invowerk-dev-account-api-openapi.yml
  format: yaml
  label: invowerk Account API
  slug: invowerk-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invowerk-dev/openapi/invowerk-dev-account-api-openapi.yml
- filename: invowerk-dev-generation-api-openapi.yml
  format: yaml
  label: invowerk Generation API
  slug: invowerk-dev-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invowerk-dev/openapi/invowerk-dev-generation-api-openapi.yml
- filename: invowerk-dev-rendering-api-openapi.yml
  format: yaml
  label: invowerk Rendering API
  slug: invowerk-dev-rendering-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invowerk-dev/openapi/invowerk-dev-rendering-api-openapi.yml
- filename: invowerk-dev-rules-api-openapi.yml
  format: yaml
  label: invowerk Rules API
  slug: invowerk-dev-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invowerk-dev/openapi/invowerk-dev-rules-api-openapi.yml
- filename: invowerk-dev-transform-api-openapi.yml
  format: yaml
  label: invowerk Transform API
  slug: invowerk-dev-transform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invowerk-dev/openapi/invowerk-dev-transform-api-openapi.yml
- filename: invowerk-dev-validation-api-openapi.yml
  format: yaml
  label: invowerk Validation API
  slug: invowerk-dev-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invowerk-dev/openapi/invowerk-dev-validation-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: invowerk.dev
  spf: true
hosts:
- cert_expires: Jan 29 05:31:18 2027 GMT
  host: invowerk.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: invowerk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for invowerk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: invowerk
provider_slug: invowerk-dev
slug: invowerk-dev-domain-security
source_filename: invowerk-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: invowerk.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 05:31:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: invowerk.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/invowerk-dev/security/invowerk-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Invoicing
- e-invoice
- PDF
- Germany
---
