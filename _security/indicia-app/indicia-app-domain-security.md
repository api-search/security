---
api_specs:
- filename: indicia-app-activity-api-openapi.yml
  format: yaml
  label: Indicia Activity API
  slug: indicia-app-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicia-app/openapi/indicia-app-activity-api-openapi.yml
- filename: indicia-app-infrastructure-api-openapi.yml
  format: yaml
  label: Indicia Infrastructure API
  slug: indicia-app-infrastructure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicia-app/openapi/indicia-app-infrastructure-api-openapi.yml
- filename: indicia-app-intelligence-api-openapi.yml
  format: yaml
  label: Indicia Intelligence API
  slug: indicia-app-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicia-app/openapi/indicia-app-intelligence-api-openapi.yml
- filename: indicia-app-organizations-api-openapi.yml
  format: yaml
  label: Indicia Organizations API
  slug: indicia-app-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicia-app/openapi/indicia-app-organizations-api-openapi.yml
- filename: indicia-app-pricing-api-openapi.yml
  format: yaml
  label: Indicia Pricing API
  slug: indicia-app-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicia-app/openapi/indicia-app-pricing-api-openapi.yml
- filename: indicia-app-socials-api-openapi.yml
  format: yaml
  label: Indicia Socials API
  slug: indicia-app-socials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicia-app/openapi/indicia-app-socials-api-openapi.yml
- filename: indicia-app-tools-api-openapi.yml
  format: yaml
  label: Indicia Tools API
  slug: indicia-app-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicia-app/openapi/indicia-app-tools-api-openapi.yml
- filename: indicia-app-unified-api-openapi.yml
  format: yaml
  label: Indicia Unified API
  slug: indicia-app-unified-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicia-app/openapi/indicia-app-unified-api-openapi.yml
- filename: indicia-app-users-api-openapi.yml
  format: yaml
  label: Indicia Users API
  slug: indicia-app-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicia-app/openapi/indicia-app-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: indicia.app
  spf: true
hosts:
- cert_expires: Feb  6 03:29:24 2027 GMT
  host: indicia.app
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Indicia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Indicia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Indicia
provider_slug: indicia-app
slug: indicia-app-domain-security
source_filename: indicia-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: indicia.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 03:29:24 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: indicia.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/indicia-app/security/indicia-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- OSINT
- Investigations
- Data Aggregation
- Cybersecurity
- Open Source
---
