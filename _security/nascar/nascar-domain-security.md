---
api_specs:
- filename: nascar-openapi.yml
  format: yaml
  label: NASCAR Feed API
  slug: nascar
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nascar/refs/heads/main/openapi/nascar-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nascar.com
  spf: true
hosts:
- cert_expires: Aug 14 10:37:49 2026 GMT
  host: www.nascar.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 16:50:05 2027 GMT
  host: feed.nascar.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Nascar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NASCAR, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NASCAR
provider_slug: nascar
slug: nascar-domain-security
source_filename: nascar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nascar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 10:37:49 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: feed.nascar.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  6 16:50:05 2027 GMT\n  hsts: false\ndomains:\n- domain: nascar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nascar/refs/heads/main/security/nascar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Auto Racing
- Sports
- Stock Cars
- Motorsports
- Race Results
- Schedules
---
