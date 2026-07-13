---
api_specs:
- filename: northflank-openapi.yml
  format: yaml
  label: Northflank API
  slug: northflank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/northflank/refs/heads/main/openapi/northflank-openapi.yml
description: ''
domains:
- caa:
  - lb.northflank.com.
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: northflank.com
  spf: true
hosts:
- cert_expires: Oct  7 16:48:48 2026 GMT
  host: northflank.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 16:48:48 2026 GMT
  host: api.northflank.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Northflank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Northflank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Northflank
provider_slug: northflank
slug: northflank-domain-security
source_filename: northflank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: northflank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 16:48:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: api.northflank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 16:48:48 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: northflank.com\n  dnssec: true\n  caa:\n  - lb.northflank.com.\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/northflank/refs/heads/main/security/northflank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cloud Deployment
- Developer Experience
- Internal Developer Platform
- Platform Engineering
---
