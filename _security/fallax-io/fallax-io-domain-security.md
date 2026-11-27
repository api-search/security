---
api_specs:
- filename: fallax-io-campaigns-api-openapi.yml
  format: yaml
  label: Fallax Campaigns API
  slug: fallax-io-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fallax-io/openapi/fallax-io-campaigns-api-openapi.yml
- filename: fallax-io-events-api-openapi.yml
  format: yaml
  label: Fallax Events API
  slug: fallax-io-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fallax-io/openapi/fallax-io-events-api-openapi.yml
- filename: fallax-io-me-api-openapi.yml
  format: yaml
  label: Fallax Me API
  slug: fallax-io-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fallax-io/openapi/fallax-io-me-api-openapi.yml
- filename: fallax-io-people-api-openapi.yml
  format: yaml
  label: Fallax People API
  slug: fallax-io-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fallax-io/openapi/fallax-io-people-api-openapi.yml
- filename: fallax-io-reports-api-openapi.yml
  format: yaml
  label: Fallax Reports API
  slug: fallax-io-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fallax-io/openapi/fallax-io-reports-api-openapi.yml
- filename: fallax-io-summary-api-openapi.yml
  format: yaml
  label: Fallax Summary API
  slug: fallax-io-summary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fallax-io/openapi/fallax-io-summary-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fallax.io
  spf: true
hosts:
- cert_expires: Feb  4 13:44:13 2027 GMT
  host: fallax.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fallax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fallax, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fallax
provider_slug: fallax-io
slug: fallax-io-domain-security
source_filename: fallax-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fallax.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 13:44:13 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fallax.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fallax-io/security/fallax-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Awareness
- Phishing
- Compliance
- Software-as-a-Service
- Company
---
