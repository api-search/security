---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: memmo.me
  spf: true
hosts:
- cert_expires: Dec 14 12:12:27 2026 GMT
  host: memmo.me
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Memmo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for memmo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: memmo
provider_slug: memmo
slug: memmo-domain-security
source_filename: memmo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memmo.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 12:12:27 2026 GMT\n  hsts: false\ndomains:\n- domain: memmo.me\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memmo/refs/heads/main/security/memmo-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Video
- Marketplace
- Celebrities
- Personalized
---
