---
api_specs:
- filename: vulk-dev-models-api-openapi.yml
  format: yaml
  label: vulk-dev Models API
  slug: vulk-dev-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vulk-dev/openapi/vulk-dev-models-api-openapi.yml
- filename: vulk-dev-operations-api-openapi.yml
  format: yaml
  label: vulk-dev Operations API
  slug: vulk-dev-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vulk-dev/openapi/vulk-dev-operations-api-openapi.yml
- filename: vulk-dev-pay-as-you-go-previous-vulk-api-openapi.yml
  format: yaml
  label: vulk-dev Pay-as-you-go (previous VULK) API
  slug: vulk-dev-pay-as-you-go-previous-vulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vulk-dev/openapi/vulk-dev-pay-as-you-go-previous-vulk-api-openapi.yml
- filename: vulk-dev-projects-api-openapi.yml
  format: yaml
  label: vulk-dev Projects API
  slug: vulk-dev-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vulk-dev/openapi/vulk-dev-projects-api-openapi.yml
- filename: vulk-dev-usage-api-openapi.yml
  format: yaml
  label: vulk-dev Usage API
  slug: vulk-dev-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vulk-dev/openapi/vulk-dev-usage-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vulk.dev
  spf: true
hosts:
- cert_expires: Dec  8 10:50:50 2026 GMT
  host: vulk.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vulk Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for vulk-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: vulk-dev
provider_slug: vulk-dev
slug: vulk-dev-domain-security
source_filename: vulk-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vulk.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 10:50:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vulk.dev\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/vulk-dev/security/vulk-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- AppBuilder
- NoCode
- 3D
---
