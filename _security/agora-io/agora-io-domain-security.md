---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "trust-provider.com"
  - 0 issue "trustasia.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "trustasia.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: agora.io
  spf: true
hosts:
- cert_expires: Dec 19 09:06:32 2026 GMT
  host: www.agora.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 09:06:32 2026 GMT
  host: docs.agora.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 09:06:32 2026 GMT
  host: api.agora.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Agora Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agora, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Agora
provider_slug: agora-io
slug: agora-io-domain-security
source_filename: agora-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agora.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 09:06:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.agora.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 09:06:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.agora.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 19 09:06:32 2026 GMT\n  hsts: null\ndomains:\n- domain: agora.io\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"trust-provider.com\"\n  - 0 issue \"trustasia.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"trustasia.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agora-io/refs/heads/main/security/agora-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Time Engagement
- Voice
- Video
- Signaling
- Conversational AI
- Streaming
- Chat
- Cloud Recording
- WebRTC
- Communications Platform
---
