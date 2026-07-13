---
api_specs:
- filename: handwrite-io-openapi.yml
  format: yaml
  label: Handwrite IO API
  slug: handwrite-io
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/handwrite-io/refs/heads/main/openapi/handwrite-io-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: handwrite.io
  spf: true
hosts:
- cert_expires: Aug 23 17:01:56 2026 GMT
  host: handwrite.io
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 15:30:22 2026 GMT
  host: documentation.handwrite.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:15:04 2026 GMT
  host: api.handwrite.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Handwrite Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Handwrite IO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Handwrite IO
provider_slug: handwrite-io
slug: handwrite-io-domain-security
source_filename: handwrite-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: handwrite.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 17:01:56 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: documentation.handwrite.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 15:30:22 2026 GMT\n  hsts: false\n- host: api.handwrite.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:15:04 2026 GMT\n  hsts: null\ndomains:\n- domain: handwrite.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/handwrite-io/refs/heads/main/security/handwrite-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Direct Mail
- Handwritten
- Marketing
- Notes
---
