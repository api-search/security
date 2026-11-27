---
api_specs:
- filename: gummble-com-api-openapi-generated.yml
  format: yaml
  label: Gummble API Reference API
  slug: api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gummble-com/openapi/_ae-authored/gummble-com-api-openapi-generated.yml
- filename: gummble-com-core-openapi-generated.yml
  format: yaml
  label: Gummble core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gummble-com/openapi/_ae-authored/gummble-com-core-openapi-generated.yml
- filename: gummble-com-mcp-openapi-generated.yml
  format: yaml
  label: Gummble MCP API
  slug: mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gummble-com/openapi/_ae-authored/gummble-com-mcp-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gummble.com
  spf: true
hosts:
- cert_expires: Feb  8 11:27:49 2027 GMT
  host: gummble.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gummble Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gummble, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gummble
provider_slug: gummble-com
slug: gummble-com-domain-security
source_filename: gummble-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gummble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 11:27:49 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gummble.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/gummble-com/security/gummble-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- UI
- Design
- Screenshots
---
