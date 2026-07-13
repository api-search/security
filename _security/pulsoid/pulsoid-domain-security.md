---
api_specs:
- filename: pulsoid-openapi.yml
  format: yaml
  label: Pulsoid
  slug: pulsoid
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/openapi/pulsoid-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pulsoid.net
  spf: false
hosts:
- cert_expires: Sep 16 04:38:57 2026 GMT
  host: pulsoid.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 17:29:23 2026 GMT
  host: docs.pulsoid.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 20:58:57 2026 GMT
  host: dev.pulsoid.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pulsoid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pulsoid, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Pulsoid
provider_slug: pulsoid
slug: pulsoid-domain-security
source_filename: pulsoid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pulsoid.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:38:57 2026 GMT\n  hsts: false\n- host: docs.pulsoid.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 17:29:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.pulsoid.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:58:57 2026 GMT\n  hsts: false\ndomains:\n- domain: pulsoid.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/security/pulsoid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Heart Rate
- Health
- Wearables
- Real-Time
- Streaming
- WebSocket
- OAuth2
---
