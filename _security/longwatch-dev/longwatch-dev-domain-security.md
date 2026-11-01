---
api_specs:
- filename: longwatch-dev-mcp-api-openapi.yml
  format: yaml
  label: longwatch-dev MCP API
  slug: longwatch-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/longwatch-dev/openapi/longwatch-dev-mcp-api-openapi.yml
- filename: longwatch-dev-website-monitoring-api-openapi.yml
  format: yaml
  label: longwatch-dev website monitoring API
  slug: longwatch-dev-website-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/longwatch-dev/openapi/longwatch-dev-website-monitoring-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: longwatch.dev
  spf: false
hosts:
- cert_expires: Dec 30 20:22:54 2026 GMT
  host: longwatch.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Longwatch Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for longwatch-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: longwatch-dev
provider_slug: longwatch-dev
slug: longwatch-dev-domain-security
source_filename: longwatch-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: longwatch.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 20:22:54 2026 GMT\n  hsts: false\ndomains:\n- domain: longwatch.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/longwatch-dev/security/longwatch-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Monitoring
- AI
- Web
- Finance
---
