---
api_specs:
- filename: traceable-platform-openapi.yml
  format: yaml
  label: Traceable Platform GraphQL API
  slug: traceable-platform-graphql
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traceable/refs/heads/main/openapi/traceable-platform-openapi.yml
- filename: traceable-platform-openapi.yml
  format: yaml
  label: Traceable API Security Platform
  slug: traceable-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/traceable/refs/heads/main/openapi/traceable-platform-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue ";"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: traceable.ai
  spf: true
hosts:
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: www.traceable.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 06:57:45 2026 GMT
  host: docs.traceable.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 07:19:11 2026 GMT
  host: api.traceable.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Traceable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Traceable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Traceable
provider_slug: traceable
slug: traceable-domain-security
source_filename: traceable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.traceable.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.traceable.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 06:57:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.traceable.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 07:19:11 2026 GMT\n  hsts: null\ndomains:\n- domain: traceable.ai\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \";\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/traceable/refs/heads/main/security/traceable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Discovery
- API Protection
- API Security
- API Testing
- Observability
- Security
- Threat Detection
---
