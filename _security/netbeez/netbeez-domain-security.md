---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: netbeez.net
  spf: true
hosts:
- cert_expires: Sep 28 16:26:00 2026 GMT
  host: netbeez.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Netbeez Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netbeez, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Netbeez
provider_slug: netbeez
slug: netbeez-domain-security
source_filename: netbeez-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: netbeez.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 16:26:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: netbeez.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netbeez/refs/heads/main/security/netbeez-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Infrastructure SaaS
- Network Monitoring
- Network Performance Monitoring
- Observability
- Wi-Fi Monitoring
- Digital Experience Monitoring
---
