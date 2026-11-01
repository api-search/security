---
api_specs:
- filename: thirdtrail-life-ephemerides-api-openapi.yml
  format: yaml
  label: thirdtrail-life Ephemerides API
  slug: thirdtrail-life-ephemerides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thirdtrail-life/openapi/thirdtrail-life-ephemerides-api-openapi.yml
- filename: thirdtrail-life-mcp-api-openapi.yml
  format: yaml
  label: thirdtrail-life MCP API
  slug: thirdtrail-life-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thirdtrail-life/openapi/thirdtrail-life-mcp-api-openapi.yml
- filename: thirdtrail-life-solar-api-openapi.yml
  format: yaml
  label: thirdtrail-life Solar API
  slug: thirdtrail-life-solar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thirdtrail-life/openapi/thirdtrail-life-solar-api-openapi.yml
- filename: thirdtrail-life-tides-api-openapi.yml
  format: yaml
  label: thirdtrail-life Tides API
  slug: thirdtrail-life-tides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thirdtrail-life/openapi/thirdtrail-life-tides-api-openapi.yml
- filename: thirdtrail-life-utility-api-openapi.yml
  format: yaml
  label: thirdtrail-life Utility API
  slug: thirdtrail-life-utility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thirdtrail-life/openapi/thirdtrail-life-utility-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thirdtrail.life
  spf: true
hosts:
- cert_expires: Jan 27 16:16:19 2027 GMT
  host: thirdtrail.life
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Thirdtrail Life Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for thirdtrail-life, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: thirdtrail-life
provider_slug: thirdtrail-life
slug: thirdtrail-life-domain-security
source_filename: thirdtrail-life-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thirdtrail.life\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 16:16:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thirdtrail.life\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/thirdtrail-life/security/thirdtrail-life-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Astronomy
- Tides
- Solar
- API
---
