---
api_specs:
- filename: livaglow-de-content-api-openapi.yml
  format: yaml
  label: LivaGlow Content API
  slug: livaglow-de-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livaglow-de/openapi/livaglow-de-content-api-openapi.yml
- filename: livaglow-de-discovery-api-openapi.yml
  format: yaml
  label: LivaGlow Discovery API
  slug: livaglow-de-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livaglow-de/openapi/livaglow-de-discovery-api-openapi.yml
- filename: livaglow-de-feeds-api-openapi.yml
  format: yaml
  label: LivaGlow Feeds API
  slug: livaglow-de-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livaglow-de/openapi/livaglow-de-feeds-api-openapi.yml
- filename: livaglow-de-mcp-api-openapi.yml
  format: yaml
  label: LivaGlow MCP API
  slug: livaglow-de-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livaglow-de/openapi/livaglow-de-mcp-api-openapi.yml
- filename: livaglow-de-status-api-openapi.yml
  format: yaml
  label: LivaGlow Status API
  slug: livaglow-de-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livaglow-de/openapi/livaglow-de-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: livaglow.de
  spf: true
hosts:
- cert_expires: Jan 19 13:47:17 2027 GMT
  host: livaglow.de
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LivaGlow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LivaGlow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: LivaGlow
provider_slug: livaglow-de
slug: livaglow-de-domain-security
source_filename: livaglow-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: livaglow.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 13:47:17 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: livaglow.de\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/livaglow-de/security/livaglow-de-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- E-Commerce
- CustomPrint
- German
- Small Business
- MugDesign
---
