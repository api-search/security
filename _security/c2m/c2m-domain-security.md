---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: connected2.me
  spf: true
hosts:
- cert_expires: Oct 12 04:40:15 2026 GMT
  host: connected2.me
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: C2M Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for C2M, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: C2M
provider_slug: c2m
slug: c2m-domain-security
source_filename: c2m-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: connected2.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:40:15 2026 GMT\n  hsts: null\ndomains:\n- domain: connected2.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/c2m/refs/heads/main/security/c2m-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Social
- Messaging
- Chat
- Mobile
- Communication
- Consumer
---
