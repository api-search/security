---
api_specs:
- filename: apigit-api.yaml
  format: yaml
  label: APIGit
  slug: apigit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apigit/refs/heads/main/openapi/apigit-api.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apigit.com
  spf: false
hosts:
- cert_expires: Sep  5 22:56:46 2026 GMT
  host: apigit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.apigit.com
  https: false
kind: domain-security
layout: security
method: probed
name: Apigit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIGit, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: APIGit
provider_slug: apigit
slug: apigit-domain-security
source_filename: apigit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apigit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 22:56:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.apigit.com\n  https: false\ndomains:\n- domain: apigit.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apigit/refs/heads/main/security/apigit-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- API Design
- API Lifecycle
- Documentation
- Git
- Governance
- Mocking
- Platform
- Testing
---
