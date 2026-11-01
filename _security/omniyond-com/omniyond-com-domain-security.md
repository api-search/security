---
api_specs:
- filename: omniyond-com-mcp-api-openapi.yml
  format: yaml
  label: omniyond-com MCP API
  slug: omniyond-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/omniyond-com/openapi/omniyond-com-mcp-api-openapi.yml
- filename: omniyond-com-scheduler-api-openapi.yml
  format: yaml
  label: omniyond-com Scheduler API
  slug: omniyond-com-scheduler-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/omniyond-com/openapi/omniyond-com-scheduler-api-openapi.yml
- filename: omniyond-com-utility-api-openapi.yml
  format: yaml
  label: omniyond-com Utility API
  slug: omniyond-com-utility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/omniyond-com/openapi/omniyond-com-utility-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: omniyond.com
  spf: true
hosts:
- cert_expires: Dec 24 20:27:33 2026 GMT
  host: omniyond.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Omniyond Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for omniyond-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: omniyond-com
provider_slug: omniyond-com
slug: omniyond-com-domain-security
source_filename: omniyond-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: omniyond.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 20:27:33 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: omniyond.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/omniyond-com/security/omniyond-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI
- API
- Pay-per-use
- Scheduling
- Automation
---
