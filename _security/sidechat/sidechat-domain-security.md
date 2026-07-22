---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sidechat.lol
  spf: true
hosts:
- cert_expires: Sep 15 14:00:51 2026 GMT
  host: sidechat.lol
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sidechat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sidechat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sidechat
provider_slug: sidechat
slug: sidechat-domain-security
source_filename: sidechat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sidechat.lol\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 14:00:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: sidechat.lol\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sidechat/refs/heads/main/security/sidechat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social
- Anonymous
- Community
- Messaging
- Consumer
- Higher Education
- Mobile
---
