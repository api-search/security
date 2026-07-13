---
api_specs:
- filename: offenders-io-openapi.yml
  format: yaml
  label: Offenders.io
  slug: offenders-io
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offenders-io/refs/heads/main/openapi/offenders-io-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: offenders.io
  spf: true
hosts:
- cert_expires: Oct  1 08:29:17 2026 GMT
  host: offenders.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 04:57:59 2026 GMT
  host: api.offenders.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Offenders Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Offenders.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Offenders.io
provider_slug: offenders-io
slug: offenders-io-domain-security
source_filename: offenders-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: offenders.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 08:29:17 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.offenders.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 04:57:59 2026 GMT\n  hsts: null\ndomains:\n- domain: offenders.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/offenders-io/refs/heads/main/security/offenders-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sex Offenders
- Public Safety
- Criminal Records
---
