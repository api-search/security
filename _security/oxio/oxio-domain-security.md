---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oxio.com
  spf: true
hosts:
- cert_expires: Oct 19 09:58:41 2026 GMT
  host: oxio.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oxio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OXIO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OXIO
provider_slug: oxio
slug: oxio-domain-security
source_filename: oxio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oxio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 09:58:41 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: oxio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oxio/refs/heads/main/security/oxio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Telecommunications
- Telecom as a Service
- MVNO
- Connectivity
- Mobile
- Networking
- Crypto Web3
---
