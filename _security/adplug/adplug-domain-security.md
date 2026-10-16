---
api_specs:
- filename: adplug-health-api-openapi.yml
  format: yaml
  label: AdPlug Health API
  slug: adplug-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/openapi/adplug-health-api-openapi.yml
- filename: adplug-mcp-api-openapi.yml
  format: yaml
  label: AdPlug MCP API
  slug: adplug-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/openapi/adplug-mcp-api-openapi.yml
- filename: adplug-oauth-api-openapi.yml
  format: yaml
  label: AdPlug OAuth API
  slug: adplug-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/openapi/adplug-oauth-api-openapi.yml
- filename: adplug-oauth-legacy-compat-api-openapi.yml
  format: yaml
  label: AdPlug OAUTH Legacy Compat API
  slug: adplug-oauth-legacy-compat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/openapi/adplug-oauth-legacy-compat-api-openapi.yml
- filename: adplug-users-api-openapi.yml
  format: yaml
  label: AdPlug Users API
  slug: adplug-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/openapi/adplug-users-api-openapi.yml
- filename: adplug-webhooks-api-openapi.yml
  format: yaml
  label: AdPlug Webhooks API
  slug: adplug-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/openapi/adplug-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adplug.app
  spf: true
hosts:
- cert_expires: Nov 14 17:56:02 2026 GMT
  host: adplug.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adplug Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AdPlug, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AdPlug
provider_slug: adplug
slug: adplug-domain-security
source_filename: adplug-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adplug.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 17:56:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: adplug.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/security/adplug-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- PPC
- AI Integration
- Agency Tools
- Search Console
---
