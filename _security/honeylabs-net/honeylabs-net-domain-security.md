---
api_specs:
- filename: honeylabs-net-bulk-api-openapi.yml
  format: yaml
  label: HoneyLabs Bulk API
  slug: honeylabs-net-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honeylabs-net/openapi/honeylabs-net-bulk-api-openapi.yml
- filename: honeylabs-net-lists-api-openapi.yml
  format: yaml
  label: HoneyLabs Lists API
  slug: honeylabs-net-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honeylabs-net/openapi/honeylabs-net-lists-api-openapi.yml
- filename: honeylabs-net-reports-api-openapi.yml
  format: yaml
  label: HoneyLabs Reports API
  slug: honeylabs-net-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honeylabs-net/openapi/honeylabs-net-reports-api-openapi.yml
- filename: honeylabs-net-service-api-openapi.yml
  format: yaml
  label: HoneyLabs Service API
  slug: honeylabs-net-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honeylabs-net/openapi/honeylabs-net-service-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: honeylabs.net
  spf: true
hosts:
- cert_expires: Jan 15 13:49:09 2027 GMT
  host: honeylabs.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HoneyLabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HoneyLabs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: HoneyLabs
provider_slug: honeylabs-net
slug: honeylabs-net-domain-security
source_filename: honeylabs-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: honeylabs.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 13:49:09 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: honeylabs.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/honeylabs-net/security/honeylabs-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Honeypot
- Threat Intelligence
- MCP
- Open Source
---
