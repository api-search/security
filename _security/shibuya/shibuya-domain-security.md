---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: shibuya.film
  spf: false
hosts:
- cert_expires: Aug 31 03:53:12 2026 GMT
  host: www.shibuya.film
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shibuya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shibuya, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Shibuya
provider_slug: shibuya
slug: shibuya-domain-security
source_filename: shibuya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shibuya.film\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 03:53:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: shibuya.film\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shibuya/refs/heads/main/security/shibuya-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Film
- Short Films
- Media
- Entertainment
- Streaming
- Creators
- Web3
---
