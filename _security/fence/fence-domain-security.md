---
api_specs:
- filename: fence-authentication-api-openapi.yml
  format: yaml
  label: Fence Authentication API
  slug: fence-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fence/openapi/fence-authentication-api-openapi.yml
- filename: fence-declaration-monitoring-api-openapi.yml
  format: yaml
  label: Fence Declaration monitoring API
  slug: fence-declaration-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fence/openapi/fence-declaration-monitoring-api-openapi.yml
- filename: fence-documents-api-openapi.yml
  format: yaml
  label: Fence Documents API
  slug: fence-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fence/openapi/fence-documents-api-openapi.yml
- filename: fence-payments-api-openapi.yml
  format: yaml
  label: Fence Payments API
  slug: fence-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fence/openapi/fence-payments-api-openapi.yml
- filename: fence-portfolio-declarations-api-openapi.yml
  format: yaml
  label: Fence Portfolio declarations API
  slug: fence-portfolio-declarations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fence/openapi/fence-portfolio-declarations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fence.finance
  spf: true
hosts:
- cert_expires: Jan 19 20:20:52 2027 GMT
  host: fence.finance
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fence
provider_slug: fence
slug: fence-domain-security
source_filename: fence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fence.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 20:20:52 2027 GMT\n  hsts: false\ndomains:\n- domain: fence.finance\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fence/security/fence-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Asset-Backed-Finance
- Real-Time
- API
---
