---
api_specs:
- filename: tokbox-openapi-generated.yml
  format: yaml
  label: TokBox API
  slug: tokbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tokbox/openapi/_ae-authored/tokbox-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tokbox.com
  spf: true
hosts:
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: tokbox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tokbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TokBox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TokBox
provider_slug: tokbox
slug: tokbox-domain-security
source_filename: tokbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tokbox.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tokbox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/tokbox/security/tokbox-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Video
- WebRTC
- Real-time Communication
- SDKs
- Vonage
---
