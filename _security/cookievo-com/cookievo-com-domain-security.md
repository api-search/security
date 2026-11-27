---
api_specs:
- filename: cookievo-com-dataset-api-openapi.yml
  format: yaml
  label: Cookievo Dataset API
  slug: cookievo-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cookievo-com/openapi/cookievo-com-dataset-api-openapi.yml
- filename: cookievo-com-mcp-api-openapi.yml
  format: yaml
  label: Cookievo MCP API
  slug: cookievo-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cookievo-com/openapi/cookievo-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cookievo.com
  spf: true
hosts:
- cert_expires: Feb  2 10:04:19 2027 GMT
  host: cookievo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cookievo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cookievo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cookievo
provider_slug: cookievo-com
slug: cookievo-com-domain-security
source_filename: cookievo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cookievo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 10:04:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cookievo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/cookievo-com/security/cookievo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Cookie Consent
- Consent Management
- Privacy
- GDPR
- Compliance
- Cookies
---
