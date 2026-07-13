---
api_specs:
- filename: meta-openapi.yml
  format: yaml
  label: Facebook Graph API - User
  slug: facebook-graph-api-user
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meta/refs/heads/main/openapi/meta-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; account=271b0beda0771d006aa3a6c11b05187d456d6c239b46cb5241196095b09c92af"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: meta.com
  spf: true
hosts:
- cert_expires: Jul 19 23:59:59 2026 GMT
  host: llama.developer.meta.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Meta
provider_slug: meta
slug: meta-domain-security
source_filename: meta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: llama.developer.meta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: meta.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; account=271b0beda0771d006aa3a6c11b05187d456d6c239b46cb5241196095b09c92af\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meta/refs/heads/main/security/meta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Analytics
- Artificial Intelligence
- Messaging
- Social
- Social Media
- Virtual Reality
---
