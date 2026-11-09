---
api_specs:
- filename: crosswire-api-com-adoption-api-openapi.yml
  format: yaml
  label: Crosswire Adoption API
  slug: crosswire-api-com-adoption-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswire-api-com/openapi/crosswire-api-com-adoption-api-openapi.yml
- filename: crosswire-api-com-audit-api-openapi.yml
  format: yaml
  label: Crosswire Audit API
  slug: crosswire-api-com-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswire-api-com/openapi/crosswire-api-com-audit-api-openapi.yml
- filename: crosswire-api-com-events-api-openapi.yml
  format: yaml
  label: Crosswire Events API
  slug: crosswire-api-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswire-api-com/openapi/crosswire-api-com-events-api-openapi.yml
- filename: crosswire-api-com-health-api-openapi.yml
  format: yaml
  label: Crosswire Health API
  slug: crosswire-api-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswire-api-com/openapi/crosswire-api-com-health-api-openapi.yml
- filename: crosswire-api-com-live-api-openapi.yml
  format: yaml
  label: Crosswire Live API
  slug: crosswire-api-com-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswire-api-com/openapi/crosswire-api-com-live-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: crosswire-api.com
  spf: false
hosts:
- cert_expires: Jan 25 16:20:13 2027 GMT
  host: crosswire-api.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crosswire Api Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crosswire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Crosswire
provider_slug: crosswire-api-com
slug: crosswire-api-com-domain-security
source_filename: crosswire-api-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crosswire-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 16:20:13 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: crosswire-api.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/crosswire-api-com/security/crosswire-api-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Finance
- Trading
- Cryptocurrency
- Risk Management
---
