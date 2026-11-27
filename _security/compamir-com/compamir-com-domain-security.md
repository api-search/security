---
api_specs:
- filename: compamir-com-conflicts-api-openapi.yml
  format: yaml
  label: COMPAMIR Conflicts API
  slug: compamir-com-conflicts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compamir-com/openapi/compamir-com-conflicts-api-openapi.yml
- filename: compamir-com-events-api-openapi.yml
  format: yaml
  label: COMPAMIR Events API
  slug: compamir-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compamir-com/openapi/compamir-com-events-api-openapi.yml
- filename: compamir-com-keys-api-openapi.yml
  format: yaml
  label: COMPAMIR Keys API
  slug: compamir-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compamir-com/openapi/compamir-com-keys-api-openapi.yml
- filename: compamir-com-meta-api-openapi.yml
  format: yaml
  label: COMPAMIR Meta API
  slug: compamir-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compamir-com/openapi/compamir-com-meta-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: compamir.com
  spf: true
hosts:
- cert_expires: Dec 12 10:31:43 2026 GMT
  host: compamir.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: COMPAMIR Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for COMPAMIR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: COMPAMIR
provider_slug: compamir-com
slug: compamir-com-domain-security
source_filename: compamir-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: compamir.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 10:31:43 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: compamir.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/compamir-com/security/compamir-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- News
- Media Monitoring
- Fact Comparison
- MCP
- AI Agents
- Japanese
- REST API
---
