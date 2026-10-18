---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: assaabloy.com
  spf: true
hosts:
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: assaabloy.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Assa Abloy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Assa Abloy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Assa Abloy
provider_slug: assa-abloy
slug: assa-abloy-domain-security
source_filename: assa-abloy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: assaabloy.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: assaabloy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/assa-abloy/refs/heads/main/security/assa-abloy-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Security
- Access Control
- IoT
- SmartBuildings
---
