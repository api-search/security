---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: floatout.xyz
  spf: true
hosts:
- cert_expires: Jan 29 04:29:41 2027 GMT
  host: floatout.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Floatout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Floatout, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Floatout
provider_slug: floatout-xyz
slug: floatout-xyz-domain-security
source_filename: floatout-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: floatout.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 04:29:41 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: floatout.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/floatout-xyz/security/floatout-xyz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Finance
- DeFi
- White Label
- Decentralized Exchange
- Cryptocurrency
---
