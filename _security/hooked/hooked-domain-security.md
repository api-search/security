---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hooked.co
  spf: true
hosts:
- cert_expires: Sep 26 06:02:21 2026 GMT
  host: hooked.co
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hooked Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hooked, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hooked
provider_slug: hooked
slug: hooked-domain-security
source_filename: hooked-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hooked.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 26 06:02:21 2026 GMT\n  hsts: false\ndomains:\n- domain: hooked.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hooked/refs/heads/main/security/hooked-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Entertainment
- Media
- Streaming
- Video
- Mobile
- Consumer
- Content
- Storytelling
---
