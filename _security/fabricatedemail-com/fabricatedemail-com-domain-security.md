---
api_specs:
- filename: fabricatedemail-com-health-api-openapi.yml
  format: yaml
  label: fabricatedemail-com Health API
  slug: fabricatedemail-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabricatedemail-com/openapi/fabricatedemail-com-health-api-openapi.yml
- filename: fabricatedemail-com-mcp-api-openapi.yml
  format: yaml
  label: fabricatedemail-com MCP API
  slug: fabricatedemail-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabricatedemail-com/openapi/fabricatedemail-com-mcp-api-openapi.yml
- filename: fabricatedemail-com-messages-api-openapi.yml
  format: yaml
  label: fabricatedemail-com Messages API
  slug: fabricatedemail-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabricatedemail-com/openapi/fabricatedemail-com-messages-api-openapi.yml
- filename: fabricatedemail-com-subscriptions-api-openapi.yml
  format: yaml
  label: fabricatedemail-com Subscriptions API
  slug: fabricatedemail-com-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabricatedemail-com/openapi/fabricatedemail-com-subscriptions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fabricatedemail.com
  spf: true
hosts:
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: fabricatedemail.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fabricatedemail Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fabricatedemail-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: fabricatedemail-com
provider_slug: fabricatedemail-com
slug: fabricatedemail-com-domain-security
source_filename: fabricatedemail-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fabricatedemail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fabricatedemail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fabricatedemail-com/security/fabricatedemail-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Email
- Disposable
- Testing
- API
- Automation
- Service
---
