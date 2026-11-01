---
api_specs:
- filename: corsproxy-dev-health-api-openapi.yml
  format: yaml
  label: corsproxy-dev Health API
  slug: corsproxy-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corsproxy-dev/openapi/corsproxy-dev-health-api-openapi.yml
- filename: corsproxy-dev-mcp-api-openapi.yml
  format: yaml
  label: corsproxy-dev MCP API
  slug: corsproxy-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corsproxy-dev/openapi/corsproxy-dev-mcp-api-openapi.yml
- filename: corsproxy-dev-proxy-api-openapi.yml
  format: yaml
  label: corsproxy-dev Proxy API
  slug: corsproxy-dev-proxy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corsproxy-dev/openapi/corsproxy-dev-proxy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: corsproxy.dev
  spf: true
hosts:
- cert_expires: Dec 13 23:04:59 2026 GMT
  host: corsproxy.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Corsproxy Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for corsproxy-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: corsproxy-dev
provider_slug: corsproxy-dev
slug: corsproxy-dev-domain-security
source_filename: corsproxy-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corsproxy.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:04:59 2026 GMT\n  hsts: false\ndomains:\n- domain: corsproxy.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/corsproxy-dev/security/corsproxy-dev-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- CORS
- Proxy
- API
- Developer Tools
- Open Source
---
