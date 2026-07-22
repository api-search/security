---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: omg.network
  spf: true
hosts:
- cert_expires: Sep 23 19:00:34 2026 GMT
  host: omg.network
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Omg Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OMG Network, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OMG Network
provider_slug: omg-network
slug: omg-network-domain-security
source_filename: omg-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: omg.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 19:00:34 2026 GMT\n  hsts: null\ndomains:\n- domain: omg.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omg-network/refs/heads/main/security/omg-network-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto
- Blockchain
- Ethereum
- Layer 2
- Plasma
- Scaling
---
