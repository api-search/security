---
api_specs:
- filename: knack-openapi.yml
  format: yaml
  label: Knack REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knack/refs/heads/main/openapi/knack-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "lencr.org"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: knack.com
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: www.knack.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 22:42:33 2026 GMT
  host: docs.knack.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  8 06:14:53 2026 GMT
  host: api.knack.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Knack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knack, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Knack
provider_slug: knack
slug: knack-domain-security
source_filename: knack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.knack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.knack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 22:42:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.knack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 06:14:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: knack.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"lencr.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knack/refs/heads/main/security/knack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- No-Code
- Database
- Application Builder
- Low-Code
- Web Applications
---
