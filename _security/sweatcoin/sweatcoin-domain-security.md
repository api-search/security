---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sweatco.in
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swe.at
  spf: true
hosts:
- cert_expires: Oct 15 20:49:17 2026 GMT
  host: sweatco.in
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 13:01:07 2026 GMT
  host: swe.at
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sweatcoin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sweatcoin, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sweatcoin
provider_slug: sweatcoin
slug: sweatcoin-domain-security
source_filename: sweatcoin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sweatco.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 20:49:17 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: swe.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 13:01:07 2026 GMT\n  hsts: false\ndomains:\n- domain: sweatco.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: swe.at\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sweatcoin/refs/heads/main/security/sweatcoin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fitness
- Health
- Wellness
- Movement
- Rewards
- Cryptocurrency
- Web3
- Consumer App
- Loyalty
---
