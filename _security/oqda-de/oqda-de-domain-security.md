---
api_specs:
- filename: oqda-de-docs-api-openapi.yml
  format: yaml
  label: oqda Docs API
  slug: oqda-de-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqda-de/openapi/oqda-de-docs-api-openapi.yml
- filename: oqda-de-katalog-api-openapi.yml
  format: yaml
  label: oqda Katalog API
  slug: oqda-de-katalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqda-de/openapi/oqda-de-katalog-api-openapi.yml
- filename: oqda-de-kontakt-api-openapi.yml
  format: yaml
  label: oqda Kontakt API
  slug: oqda-de-kontakt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqda-de/openapi/oqda-de-kontakt-api-openapi.yml
- filename: oqda-de-mcp-api-openapi.yml
  format: yaml
  label: oqda MCP API
  slug: oqda-de-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqda-de/openapi/oqda-de-mcp-api-openapi.yml
- filename: oqda-de-oqda-api-api-openapi.yml
  format: yaml
  label: oqda Oqda API
  slug: oqda-de-oqda-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqda-de/openapi/oqda-de-oqda-api-api-openapi.yml
- filename: oqda-de-warteliste-api-openapi.yml
  format: yaml
  label: oqda Warteliste API
  slug: oqda-de-warteliste-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqda-de/openapi/oqda-de-warteliste-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oqda.de
  spf: true
hosts:
- cert_expires: Dec 28 06:22:59 2026 GMT
  host: oqda.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: oqda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for oqda, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: oqda
provider_slug: oqda-de
slug: oqda-de-domain-security
source_filename: oqda-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oqda.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 06:22:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oqda.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/oqda-de/security/oqda-de-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business-OS
- Scheduling
- AI Assistant
- GDPR
- Germany
---
