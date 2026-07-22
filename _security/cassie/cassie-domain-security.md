---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aircassie.com
  spf: false
hosts:
- cert_expires: Aug 26 23:48:23 2026 GMT
  host: aircassie.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cassie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cassie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Cassie
provider_slug: cassie
slug: cassie-domain-security
source_filename: cassie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aircassie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 23:48:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: aircassie.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cassie/refs/heads/main/security/cassie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Air Filtration
- Air Quality
- Healthcare
- Environmental Technology
- Hardware
- Air Quality Monitoring
- Medical Devices
---
