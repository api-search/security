---
api_specs:
- filename: 409acost-com-calculator-api-openapi.yml
  format: yaml
  label: 409A Cost Calculator API
  slug: 409acost-com-calculator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/409acost-com/openapi/409acost-com-calculator-api-openapi.yml
- filename: 409acost-com-enquiry-api-openapi.yml
  format: yaml
  label: 409A Cost Enquiry API
  slug: 409acost-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/409acost-com/openapi/409acost-com-enquiry-api-openapi.yml
- filename: 409acost-com-mcp-api-openapi.yml
  format: yaml
  label: 409A Cost MCP API
  slug: 409acost-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/409acost-com/openapi/409acost-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 409acost.com
  spf: true
hosts:
- cert_expires: Jan 10 12:14:06 2027 GMT
  host: 409acost.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 409Acost Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 409A Cost, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 409A Cost
provider_slug: 409acost-com
slug: 409acost-com-domain-security
source_filename: 409acost-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 409acost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 12:14:06 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 409acost.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/409acost-com/security/409acost-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Valuation
- Startups
- Finance
- Calculator
---
