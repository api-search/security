---
api_specs:
- filename: fundamentwebb-se-company-api-openapi.yml
  format: yaml
  label: Fundament Company API
  slug: fundamentwebb-se-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundamentwebb-se/openapi/fundamentwebb-se-company-api-openapi.yml
- filename: fundamentwebb-se-financials-api-openapi.yml
  format: yaml
  label: Fundament Financials API
  slug: fundamentwebb-se-financials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundamentwebb-se/openapi/fundamentwebb-se-financials-api-openapi.yml
- filename: fundamentwebb-se-free-api-openapi.yml
  format: yaml
  label: Fundament Free API
  slug: fundamentwebb-se-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fundamentwebb-se/openapi/fundamentwebb-se-free-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fundamentwebb.se
  spf: true
hosts:
- cert_expires: Jan  3 12:44:39 2027 GMT
  host: fundamentwebb.se
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fundament Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fundament, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fundament
provider_slug: fundamentwebb-se
slug: fundamentwebb-se-domain-security
source_filename: fundamentwebb-se-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fundamentwebb.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 12:44:39 2027 GMT\n  hsts: false\ndomains:\n- domain: fundamentwebb.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fundamentwebb-se/security/fundamentwebb-se-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- WebAgency
- Web Design
- Small Business
- Sweden
- Jönköping
---
