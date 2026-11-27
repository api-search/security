---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: manifest.network
  spf: true
hosts:
- cert_expires: Feb  5 14:40:35 2027 GMT
  host: manifest.network
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Manifest Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Manifest Network, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Manifest Network
provider_slug: manifest-network
slug: manifest-network-domain-security
source_filename: manifest-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: manifest.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 14:40:35 2027 GMT\n  hsts: null\ndomains:\n- domain: manifest.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/manifest-network/security/manifest-network-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Web3
- Decentralization
- Ethics
- Community
---
