---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: friend.tech
  spf: true
hosts:
- cert_expires: Oct  8 12:55:48 2026 GMT
  host: www.friend.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Friendtech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Friend.tech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Friend.tech
provider_slug: friendtech
slug: friendtech-domain-security
source_filename: friendtech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.friend.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 12:55:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: friend.tech\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/friendtech/refs/heads/main/security/friendtech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Social
- Web3
- Blockchain
- Base
- Social
- DeFi
---
