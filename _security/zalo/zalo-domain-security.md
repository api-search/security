---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zalo.me
  spf: true
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: zalo.me
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zalo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zalo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zalo
provider_slug: zalo
slug: zalo-domain-security
source_filename: zalo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zalo.me\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: zalo.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zalo/refs/heads/main/security/zalo-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Messaging
- CPaaS
- Vietnam
- Notification
---
