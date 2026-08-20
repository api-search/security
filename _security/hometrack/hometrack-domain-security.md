---
api_specs:
- filename: hometrack-broker-avm-api-openapi.yml
  format: yaml
  label: Hometrack Broker AVM API
  slug: hometrack-broker-avm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-broker-avm-api-openapi.yml
- filename: hometrack-climate-graphql-api-openapi.yml
  format: yaml
  label: Hometrack Climate GraphQL API
  slug: hometrack-climate-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-climate-graphql-api-openapi.yml
- filename: hometrack-api-public-openapi.yml
  format: yaml
  label: Hometrack API Public
  slug: hometrack-api-public-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-api-public-openapi.yml
- filename: hometrack-climate-api-v2-openapi.yml
  format: yaml
  label: Hometrack Climate API (v2)
  slug: hometrack-climate-api-v2-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-climate-api-v2-openapi.yml
- filename: hometrack-prh-core-external-client-api-v2-openapi.yml
  format: yaml
  label: Hometrack (PRH) - Core External Client API v2.0
  slug: hometrack-prh-core-external-client-api-v2-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-prh-core-external-client-api-v2-openapi.yml
- filename: hometrack-valuation-api-v1-openapi.yml
  format: yaml
  label: Hometrack Valuation API
  slug: hometrack-valuation-api-v1-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-valuation-api-v1-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hometrack.com
  spf: true
hosts:
- cert_expires: Oct 21 18:23:34 2026 GMT
  host: www.hometrack.com
  hsts: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: developer.hometrack.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: api.hometrack.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hometrack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hometrack, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hometrack
provider_slug: hometrack
slug: hometrack-domain-security
source_filename: hometrack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hometrack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 18:23:34 2026 GMT\n  hsts: true\n- host: developer.hometrack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.hometrack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hometrack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/security/hometrack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- United Kingdom
- PropTech
- Valuation
- AVM
- Mortgage
- Property Data
- Climate Risk
- Lending
- Surveying
---
