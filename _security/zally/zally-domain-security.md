---
api_specs:
- filename: zally-api.yml
  format: yaml
  label: Zally API
  slug: zally-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zally/refs/heads/main/openapi/zally-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zalando.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: inter.net
  spf: true
hosts:
- cert_expires: Sep 28 21:17:50 2026 GMT
  host: opensource.zalando.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: zally.on.inter.net
  https: false
kind: domain-security
layout: security
method: probed
name: Zally Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zally, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zally
provider_slug: zally
slug: zally-domain-security
source_filename: zally-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opensource.zalando.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 21:17:50 2026 GMT\n  hsts: false\n- host: zally.on.inter.net\n  https: false\ndomains:\n- domain: zalando.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: inter.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zally/refs/heads/main/security/zally-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Design
- API Linting
- API Quality
- Open Source
- OpenAPI
- Zalando
---
