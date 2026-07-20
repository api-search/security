---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: harmonicinc.com
  spf: true
hosts:
- cert_expires: Oct 16 17:21:57 2026 GMT
  host: harmonicinc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Harmonicinc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harmonic Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Harmonic Inc.
provider_slug: harmonicinc
slug: harmonicinc-domain-security
source_filename: harmonicinc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: harmonicinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 17:21:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: harmonicinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harmonicinc/refs/heads/main/security/harmonicinc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Video
- Video Streaming
- Broadband
- Media
- Streaming
- SaaS
- Telecommunications
---
