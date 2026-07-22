---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: peer39.com
  spf: true
hosts:
- cert_expires: Sep 14 01:28:08 2026 GMT
  host: www.peer39.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peer39 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peer39, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Peer39
provider_slug: peer39
slug: peer39-domain-security
source_filename: peer39-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.peer39.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 01:28:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: peer39.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peer39/refs/heads/main/security/peer39-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Contextual Advertising
- AdTech
- Brand Safety
- Programmatic Advertising
- Contextual Targeting
- CTV
- MarTech
---
