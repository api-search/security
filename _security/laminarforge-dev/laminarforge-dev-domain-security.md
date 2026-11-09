---
api_specs:
- filename: laminarforge-dev-format-utils-api-openapi.yml
  format: yaml
  label: LaminarForge API Format Utils API
  slug: laminarforge-dev-format-utils-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/laminarforge-dev/openapi/laminarforge-dev-format-utils-api-openapi.yml
- filename: laminarforge-dev-platform-api-openapi.yml
  format: yaml
  label: LaminarForge API Platform API
  slug: laminarforge-dev-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/laminarforge-dev/openapi/laminarforge-dev-platform-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: laminarforge.dev
  spf: false
hosts:
- cert_expires: Jan  9 14:23:03 2027 GMT
  host: laminarforge.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Laminarforge Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LaminarForge API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LaminarForge API
provider_slug: laminarforge-dev
slug: laminarforge-dev-domain-security
source_filename: laminarforge-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: laminarforge.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 14:23:03 2027 GMT\n  hsts: false\ndomains:\n- domain: laminarforge.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/laminarforge-dev/security/laminarforge-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- API Marketplace
- Utilities
- Developer Tools
- Integration
- Cloud Services
---
