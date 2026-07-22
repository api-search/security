---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: royal.io
  spf: true
hosts:
- cert_expires: Sep 28 11:18:43 2026 GMT
  host: royal.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Royal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Royal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Royal
provider_slug: royal
slug: royal-domain-security
source_filename: royal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: royal.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 11:18:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: royal.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/royal/refs/heads/main/security/royal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Music
- Royalties
- Crypto
- Web3
- NFT
- Fan Engagement
---
