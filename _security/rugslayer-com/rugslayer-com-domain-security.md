---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rugslayer.com
  spf: true
hosts:
- cert_expires: Jan 22 02:50:23 2027 GMT
  host: rugslayer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rugslayer Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for rugslayer-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: rugslayer-com
provider_slug: rugslayer-com
slug: rugslayer-com-domain-security
source_filename: rugslayer-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rugslayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 02:50:23 2027 GMT\n  hsts: false\ndomains:\n- domain: rugslayer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/rugslayer-com/security/rugslayer-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Solana
- Security
- Crypto
- Risk-Scanner
---
