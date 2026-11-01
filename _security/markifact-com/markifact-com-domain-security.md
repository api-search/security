---
api_specs:
- filename: markifact-com-connections-api-openapi.yml
  format: yaml
  label: markifact-com Connections API
  slug: markifact-com-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/markifact-com/openapi/markifact-com-connections-api-openapi.yml
- filename: markifact-com-credits-api-openapi.yml
  format: yaml
  label: markifact-com Credits API
  slug: markifact-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/markifact-com/openapi/markifact-com-credits-api-openapi.yml
- filename: markifact-com-logs-api-openapi.yml
  format: yaml
  label: markifact-com Logs API
  slug: markifact-com-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/markifact-com/openapi/markifact-com-logs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: markifact.com
  spf: true
hosts:
- cert_expires: Jan 18 22:33:55 2027 GMT
  host: markifact.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Markifact Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for markifact-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: markifact-com
provider_slug: markifact-com
slug: markifact-com-domain-security
source_filename: markifact-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: markifact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 22:33:55 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: markifact.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/markifact-com/security/markifact-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Marketing Automation
- Ad Management
- Reporting
- Workflow Automation
- Marketing Operations
- Data Integration
---
