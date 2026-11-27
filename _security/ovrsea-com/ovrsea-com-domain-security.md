---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ovrsea.com
  spf: true
hosts:
- cert_expires: Feb 10 13:46:55 2027 GMT
  host: ovrsea.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OVRSEA Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OVRSEA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OVRSEA
provider_slug: ovrsea-com
slug: ovrsea-com-domain-security
source_filename: ovrsea-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ovrsea.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 13:46:55 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ovrsea.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ovrsea-com/security/ovrsea-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logistics
- Freight
- Artificial Intelligence
- Supply Chain
- Transport
---
