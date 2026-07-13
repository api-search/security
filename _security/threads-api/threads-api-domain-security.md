---
api_specs:
- filename: threads-api-openapi.yml
  format: yaml
  label: Threads API
  slug: threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threads-api/refs/heads/main/openapi/threads-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; account=271b0beda0771d006aa3a6c11b05187d456d6c239b46cb5241196095b09c92af"
  dmarc: false
  dnssec: false
  domain: threads.net
  spf: true
hosts:
- cert_expires: Jul 19 23:59:59 2026 GMT
  host: www.threads.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 19 23:59:59 2026 GMT
  host: graph.threads.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Threads Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Threads, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Threads
provider_slug: threads-api
slug: threads-api-domain-security
source_filename: threads-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.threads.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: graph.threads.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: threads.net\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; account=271b0beda0771d006aa3a6c11b05187d456d6c239b46cb5241196095b09c92af\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/threads-api/refs/heads/main/security/threads-api-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Social
- Social Networks
- Meta
- Publishing
- Media
---
