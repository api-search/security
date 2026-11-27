---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ipdefender.eu
  spf: true
hosts:
- cert_expires: Jan  7 16:41:36 2027 GMT
  host: ipdefender.eu
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IP Defender Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IP Defender, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: IP Defender
provider_slug: ipdefender-eu
slug: ipdefender-eu-domain-security
source_filename: ipdefender-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ipdefender.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 16:41:36 2027 GMT\n  hsts: null\ndomains:\n- domain: ipdefender.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ipdefender-eu/security/ipdefender-eu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Trademarks
- Monitoring
- Brand Protection
- Artificial Intelligence
- Software-as-a-Service
---
