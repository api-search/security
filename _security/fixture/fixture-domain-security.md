---
api_specs:
- filename: fixture-v1-openapi.json
  format: json
  label: Fixture API v1
  slug: fixture-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fixture.app
  spf: true
hosts:
- cert_expires: Aug 23 12:56:41 2026 GMT
  host: fixture.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 10:14:41 2026 GMT
  host: beta-api.fixture.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fixture Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fixture, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fixture
provider_slug: fixture
slug: fixture-domain-security
source_filename: fixture-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fixture.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 12:56:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: beta-api.fixture.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 10:14:41 2026 GMT\n  hsts: null\ndomains:\n- domain: fixture.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/security/fixture-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- CRM
- Sales
- B2B
- Artificial Intelligence
- Agents
- MCP
- Customer Relationship Management
---
