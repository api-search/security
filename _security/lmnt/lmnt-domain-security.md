---
api_specs:
- filename: lmnt-speech-openapi.yml
  format: yaml
  label: LMNT Speech API
  slug: lmnt-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lmnt/refs/heads/main/openapi/lmnt-speech-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lmnt.com
  spf: true
hosts:
- cert_expires: Sep  3 07:00:38 2026 GMT
  host: www.lmnt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 09:31:36 2026 GMT
  host: docs.lmnt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 01:35:53 2026 GMT
  host: api.lmnt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lmnt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LMNT, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: LMNT
provider_slug: lmnt
slug: lmnt-domain-security
source_filename: lmnt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lmnt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 07:00:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.lmnt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 09:31:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.lmnt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 01:35:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lmnt.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lmnt/refs/heads/main/security/lmnt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- text-to-speech
- voice synthesis
- voice cloning
- audio streaming
- conversational AI
- low latency
- real-time audio
---
