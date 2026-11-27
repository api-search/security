---
api_specs:
- filename: fieldstub-com-links-api-openapi.yml
  format: yaml
  label: Fieldstub Links API
  slug: fieldstub-com-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fieldstub-com/openapi/fieldstub-com-links-api-openapi.yml
- filename: fieldstub-com-projects-api-openapi.yml
  format: yaml
  label: Fieldstub Projects API
  slug: fieldstub-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fieldstub-com/openapi/fieldstub-com-projects-api-openapi.yml
- filename: fieldstub-com-tickets-api-openapi.yml
  format: yaml
  label: Fieldstub Tickets API
  slug: fieldstub-com-tickets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fieldstub-com/openapi/fieldstub-com-tickets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fieldstub.com
  spf: true
hosts:
- cert_expires: Jan  5 00:48:28 2027 GMT
  host: fieldstub.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fieldstub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fieldstub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fieldstub
provider_slug: fieldstub-com
slug: fieldstub-com-domain-security
source_filename: fieldstub-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fieldstub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 00:48:28 2027 GMT\n  hsts: false\ndomains:\n- domain: fieldstub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fieldstub-com/security/fieldstub-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Construction
- Field Service Management
- Procore Integration
- Time and Materials
- NoLogin
---
