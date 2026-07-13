---
api_specs:
- filename: coderabbit-openapi.yml
  format: yaml
  label: CodeRabbit Reports API
  slug: coderabbit-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coderabbit/refs/heads/main/openapi/coderabbit-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coderabbit.ai
  spf: true
hosts:
- cert_expires: Oct  4 02:03:50 2026 GMT
  host: www.coderabbit.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 12:48:56 2026 GMT
  host: docs.coderabbit.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 17:10:07 2026 GMT
  host: api.coderabbit.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coderabbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodeRabbit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CodeRabbit
provider_slug: coderabbit
slug: coderabbit-domain-security
source_filename: coderabbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coderabbit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 02:03:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.coderabbit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 12:48:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.coderabbit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 17:10:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: coderabbit.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coderabbit/refs/heads/main/security/coderabbit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Code Review
- Developer Tools
- Pull Requests
- DevOps
---
