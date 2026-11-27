---
api_specs:
- filename: glyt-net-receipts-api-openapi.yml
  format: yaml
  label: Glyt Receipts API
  slug: glyt-net-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glyt-net/openapi/glyt-net-receipts-api-openapi.yml
- filename: glyt-net-requests-api-openapi.yml
  format: yaml
  label: Glyt Requests API
  slug: glyt-net-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glyt-net/openapi/glyt-net-requests-api-openapi.yml
- filename: glyt-net-verify-api-openapi.yml
  format: yaml
  label: Glyt Verify API
  slug: glyt-net-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glyt-net/openapi/glyt-net-verify-api-openapi.yml
- filename: glyt-net-well-known-api-openapi.yml
  format: yaml
  label: Glyt .well Known API
  slug: glyt-net-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glyt-net/openapi/glyt-net-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: glyt.net
  spf: true
hosts:
- cert_expires: Jan 19 14:13:11 2027 GMT
  host: glyt.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Glyt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glyt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Glyt
provider_slug: glyt-net
slug: glyt-net-domain-security
source_filename: glyt-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glyt.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 14:13:11 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: glyt.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/glyt-net/security/glyt-net-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Human-in-the-Loop
- Agent-Approval
- Security
- Automation
---
