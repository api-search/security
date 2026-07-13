---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Basis Enterprise API
  slug: basis-enterprise-api
  spec_type: OpenAPI
  url: https://api.basis.net/docs/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: basis.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: basis.net
  spf: true
hosts:
- cert_expires: Aug 23 15:53:27 2026 GMT
  host: basis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: api.basis.net
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Basis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Basis, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Basis
provider_slug: basis
slug: basis-domain-security
source_filename: basis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: basis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 15:53:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.basis.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: basis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: basis.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basis/refs/heads/main/security/basis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Programmatic Advertising
- DSP
- Media Buying
- Campaign Management
- Audience Targeting
- AdTech
---
