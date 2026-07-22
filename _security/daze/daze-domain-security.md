---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: daze.chat
  spf: true
hosts:
- cert_expires: Sep 15 18:46:08 2026 GMT
  host: daze.chat
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Daze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daze, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Daze
provider_slug: daze
slug: daze-domain-security
source_filename: daze-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: daze.chat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 18:46:08 2026 GMT\n  hsts: false\ndomains:\n- domain: daze.chat\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daze/refs/heads/main/security/daze-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Chat
- Messaging
- Social
- Mobile
- Consumer
---
