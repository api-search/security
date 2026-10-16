---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cartame.by
  spf: true
hosts:
- cert_expires: Nov 25 04:07:01 2026 GMT
  host: cartame.by
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cartame Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cartame, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cartame
provider_slug: cartame
slug: cartame-domain-security
source_filename: cartame-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cartame.by\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 04:07:01 2026 GMT\n  hsts: false\ndomains:\n- domain: cartame.by\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cartame/refs/heads/main/security/cartame-domain-security.yml
summary_line: TLSv1.3
tags:
- Loyalty
- Rewards
- Retail
- MobileApp
---
