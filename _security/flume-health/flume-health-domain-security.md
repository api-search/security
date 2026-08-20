---
api_specs:
- filename: flume-health-console-api-openapi.yml
  format: yaml
  label: Flume Console API
  slug: flume-console-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-console-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: flumehealth.com
  spf: true
hosts:
- cert_expires: Oct 10 14:37:33 2026 GMT
  host: www.flumehealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 17:13:25 2026 GMT
  host: console.flumehealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flume Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flume Health, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Flume Health
provider_slug: flume-health
slug: flume-health-domain-security
source_filename: flume-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flumehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 14:37:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: console.flumehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 17:13:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flumehealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/security/flume-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- Health Plans
- Payers
- Healthcare Data
- Data Integration
- iPaaS
- Eligibility
- Claims
- Knowledge Graph
- MCP
- agent-native
- Authentication
- Data Engineering
- Interoperability
---
