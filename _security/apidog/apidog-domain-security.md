---
api_specs:
- filename: apidog-apidog-openapi.yml
  format: yaml
  label: Apidog
  slug: apidog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apidog/refs/heads/main/openapi/apidog-apidog-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: apidog.com
  spf: true
hosts:
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: apidog.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: api.apidog.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apidog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apidog, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Apidog
provider_slug: apidog
slug: apidog-domain-security
source_filename: apidog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apidog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.apidog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: apidog.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apidog/refs/heads/main/security/apidog-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Coding
- API Design
- API Lifecycle
- API Testing
- Collaboration
- Design-First
- Documentation
- MCP
- Mocking
- Platform
---
