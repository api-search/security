---
api_specs:
- filename: wallarm-openapi.yml
  format: yaml
  label: Wallarm API
  slug: wallarm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallarm/refs/heads/main/openapi/wallarm-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wallarm.com
  spf: true
hosts:
- cert_expires: Aug 15 19:15:29 2026 GMT
  host: www.wallarm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 15:31:29 2026 GMT
  host: docs.wallarm.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 13:29:19 2026 GMT
  host: us1.api.wallarm.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wallarm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wallarm, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wallarm
provider_slug: wallarm
slug: wallarm-domain-security
source_filename: wallarm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wallarm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 19:15:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.wallarm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 15:31:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: us1.api.wallarm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 13:29:19 2026 GMT\n  hsts: null\ndomains:\n- domain: wallarm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wallarm/refs/heads/main/security/wallarm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Security
- Security Testing
- WAF
- Cybersecurity
---
