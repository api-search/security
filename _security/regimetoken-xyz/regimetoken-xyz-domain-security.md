---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: false
  domain: regimetoken.xyz
  spf: false
hosts:
- cert_expires: Jan 23 08:49:11 2027 GMT
  host: regimetoken.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Regime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Regime, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Regime
provider_slug: regimetoken-xyz
slug: regimetoken-xyz-domain-security
source_filename: regimetoken-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: regimetoken.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 08:49:11 2027 GMT\n  hsts: false\ndomains:\n- domain: regimetoken.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/regimetoken-xyz/security/regimetoken-xyz-domain-security.yml
summary_line: TLSv1.3
tags:
- Cryptocurrency
- Analytics
- Tools
- OpenData
- Community
---
