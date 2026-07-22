---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jiayuan.com
  spf: true
hosts:
- cert_expires: Nov 27 02:37:19 2026 GMT
  host: jiayuan.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jiayuan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for jiayuan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: jiayuan
provider_slug: jiayuan
slug: jiayuan-domain-security
source_filename: jiayuan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jiayuan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 02:37:19 2026 GMT\n  hsts: false\ndomains:\n- domain: jiayuan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jiayuan/refs/heads/main/security/jiayuan-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Online Dating
- Matchmaking
- Social
- Consumer
- China
- Relationships
---
