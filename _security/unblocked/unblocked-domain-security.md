---
api_specs:
- filename: unblocked-public-api-openapi-original.json
  format: json
  label: Unblocked Public API
  slug: unblocked-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unblocked/refs/heads/main/openapi/unblocked-public-api-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: getunblocked.com
  spf: true
hosts:
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: getunblocked.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unblocked Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unblocked, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Unblocked
provider_slug: unblocked
slug: unblocked-domain-security
source_filename: unblocked-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getunblocked.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: getunblocked.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unblocked/refs/heads/main/security/unblocked-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Developer Tools
- AI
- Developer Experience
- Knowledge Management
- Code Review
- MCP
- AI Agents
- Context Engineering
- Search
---
