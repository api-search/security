---
api_specs:
- filename: matter-openapi-original.yml
  format: yaml
  label: Matter API
  slug: matter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matter/refs/heads/main/openapi/matter-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getmatter.app
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getmatter.com
  spf: false
hosts:
- cert_expires: Sep  7 07:54:31 2026 GMT
  host: getmatter.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: api.getmatter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Matter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Matter, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Matter
provider_slug: matter
slug: matter-domain-security
source_filename: matter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getmatter.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 07:54:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getmatter.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getmatter.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: getmatter.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matter/refs/heads/main/security/matter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Reading
- Read Later
- Productivity
- Content
- Highlights
- Bookmarking
---
