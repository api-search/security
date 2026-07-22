---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: odyssey.world
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: odyssey.ml
  spf: true
hosts:
- cert_expires: Oct 10 19:54:56 2026 GMT
  host: odyssey.world
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 02:18:42 2026 GMT
  host: documentation.api.odyssey.ml
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 19:46:33 2026 GMT
  host: api.odyssey.ml
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Odyssey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Odyssey, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Odyssey
provider_slug: odyssey
slug: odyssey-domain-security
source_filename: odyssey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: odyssey.world\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 19:54:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: documentation.api.odyssey.ml\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 02:18:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.odyssey.ml\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 19:46:33 2026 GMT\n  hsts: null\ndomains:\n- domain: odyssey.world\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: odyssey.ml\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/odyssey/refs/heads/main/security/odyssey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- World Models
- Generative AI
- Video Generation
- Machine Learning
- Real-Time Streaming
- SDK
- WebRTC
---
