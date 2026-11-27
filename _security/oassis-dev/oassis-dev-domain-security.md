---
api_specs:
- filename: oassis-dev-account-api-openapi.yml
  format: yaml
  label: Oassis Account API
  slug: oassis-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oassis-dev/openapi/oassis-dev-account-api-openapi.yml
- filename: oassis-dev-agents-api-openapi.yml
  format: yaml
  label: Oassis Agents API
  slug: oassis-dev-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oassis-dev/openapi/oassis-dev-agents-api-openapi.yml
- filename: oassis-dev-discovery-api-openapi.yml
  format: yaml
  label: Oassis Discovery API
  slug: oassis-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oassis-dev/openapi/oassis-dev-discovery-api-openapi.yml
- filename: oassis-dev-web-tasks-api-openapi.yml
  format: yaml
  label: Oassis Web Tasks API
  slug: oassis-dev-web-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oassis-dev/openapi/oassis-dev-web-tasks-api-openapi.yml
- filename: oassis-dev-web-tools-api-openapi.yml
  format: yaml
  label: Oassis Web Tools API
  slug: oassis-dev-web-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oassis-dev/openapi/oassis-dev-web-tools-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oassis.dev
  spf: true
hosts:
- cert_expires: Dec 28 20:22:20 2026 GMT
  host: oassis.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Oassis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oassis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Oassis
provider_slug: oassis-dev
slug: oassis-dev-domain-security
source_filename: oassis-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oassis.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 20:22:20 2026 GMT\n  hsts: false\ndomains:\n- domain: oassis.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/oassis-dev/security/oassis-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Web Scraping
- Browser Automation
- AI Agents
- MCP
---
