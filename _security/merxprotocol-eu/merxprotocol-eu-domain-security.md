---
api_specs:
- filename: merxprotocol-eu-company-api-openapi.yml
  format: yaml
  label: Merx Company API
  slug: merxprotocol-eu-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merxprotocol-eu/openapi/merxprotocol-eu-company-api-openapi.yml
- filename: merxprotocol-eu-discovery-api-openapi.yml
  format: yaml
  label: Merx Discovery API
  slug: merxprotocol-eu-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merxprotocol-eu/openapi/merxprotocol-eu-discovery-api-openapi.yml
- filename: merxprotocol-eu-legal-api-openapi.yml
  format: yaml
  label: Merx Legal API
  slug: merxprotocol-eu-legal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merxprotocol-eu/openapi/merxprotocol-eu-legal-api-openapi.yml
- filename: merxprotocol-eu-vat-api-openapi.yml
  format: yaml
  label: Merx VAT API
  slug: merxprotocol-eu-vat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merxprotocol-eu/openapi/merxprotocol-eu-vat-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: merxprotocol.eu
  spf: true
hosts:
- cert_expires: Dec 25 06:05:07 2026 GMT
  host: merxprotocol.eu
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Merx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Merx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Merx
provider_slug: merxprotocol-eu
slug: merxprotocol-eu-domain-security
source_filename: merxprotocol-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: merxprotocol.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 06:05:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: merxprotocol.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/merxprotocol-eu/security/merxprotocol-eu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Agentic Commerce
- European Services
- Directory
---
