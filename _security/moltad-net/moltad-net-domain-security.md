---
api_specs:
- filename: moltad-net-agent-api-openapi.yml
  format: yaml
  label: MoltAd Agent API
  slug: moltad-net-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moltad-net/openapi/moltad-net-agent-api-openapi.yml
- filename: moltad-net-mcp-api-openapi.yml
  format: yaml
  label: MoltAd MCP API
  slug: moltad-net-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moltad-net/openapi/moltad-net-mcp-api-openapi.yml
- filename: moltad-net-placements-api-openapi.yml
  format: yaml
  label: MoltAd Placements API
  slug: moltad-net-placements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moltad-net/openapi/moltad-net-placements-api-openapi.yml
- filename: moltad-net-public-api-openapi.yml
  format: yaml
  label: MoltAd Public API
  slug: moltad-net-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moltad-net/openapi/moltad-net-public-api-openapi.yml
- filename: moltad-net-webhooks-api-openapi.yml
  format: yaml
  label: MoltAd Webhooks API
  slug: moltad-net-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moltad-net/openapi/moltad-net-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: moltad.net
  spf: true
hosts:
- cert_expires: Jan  3 20:07:11 2027 GMT
  host: moltad.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MoltAd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MoltAd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MoltAd
provider_slug: moltad-net
slug: moltad-net-domain-security
source_filename: moltad-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moltad.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 20:07:11 2027 GMT\n  hsts: false\ndomains:\n- domain: moltad.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/moltad-net/security/moltad-net-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Advertising
- Artificial Intelligence
- Publishers
- Advertisers
- Leads
- Shopping
- Chat
- XML/CPC
---
