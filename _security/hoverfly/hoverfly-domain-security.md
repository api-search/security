---
api_specs:
- filename: hoverfly-openapi.yml
  format: yaml
  label: Hoverfly Admin API
  slug: hoverfly-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hoverfly/refs/heads/main/openapi/hoverfly-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: hoverfly.io
  spf: true
hosts:
- cert_expires: Aug 25 11:45:10 2026 GMT
  host: hoverfly.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 12:13:04 2026 GMT
  host: docs.hoverfly.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hoverfly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hoverfly, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Hoverfly
provider_slug: hoverfly
slug: hoverfly-domain-security
source_filename: hoverfly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hoverfly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 11:45:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.hoverfly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:13:04 2026 GMT\n  hsts: false\ndomains:\n- domain: hoverfly.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hoverfly/refs/heads/main/security/hoverfly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Mocking
- Testing
---
