---
api_specs:
- filename: getgenko-com-analytics-api-openapi.yml
  format: yaml
  label: Genkō Analytics API
  slug: getgenko-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getgenko-com/openapi/getgenko-com-analytics-api-openapi.yml
- filename: getgenko-com-mcp-api-openapi.yml
  format: yaml
  label: Genkō MCP API
  slug: getgenko-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getgenko-com/openapi/getgenko-com-mcp-api-openapi.yml
- filename: getgenko-com-risk-api-openapi.yml
  format: yaml
  label: Genkō Risk API
  slug: getgenko-com-risk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getgenko-com/openapi/getgenko-com-risk-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:security@getenko.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getgenko.com
  spf: true
hosts:
- cert_expires: Feb  3 22:11:14 2027 GMT
  host: getgenko.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Genkō Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genkō, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Genkō
provider_slug: getgenko-com
slug: getgenko-com-domain-security
source_filename: getgenko-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getgenko.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 22:11:14 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getgenko.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:security@getenko.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getgenko-com/security/getgenko-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Scheduling
- Electronic Health Records
- Software-as-a-Service
- Clinics
---
