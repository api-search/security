---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: figuremarkets.com
  spf: true
hosts:
- cert_expires: Aug 31 15:37:39 2026 GMT
  host: figuremarkets.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Figure Markets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Figure Markets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Figure Markets
provider_slug: figure-markets
slug: figure-markets-domain-security
source_filename: figure-markets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: figuremarkets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 15:37:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: figuremarkets.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/figure-markets/refs/heads/main/security/figure-markets-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Cryptocurrency
- Digital Assets
- Exchange
- Trading
- Blockchain
- Lending
- Stablecoin
- Provenance Blockchain
---
