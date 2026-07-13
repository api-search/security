---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aisgroup.com
  spf: true
hosts:
- cert_expires: Oct  4 02:02:16 2026 GMT
  host: www.aisgroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 19:14:09 2026 GMT
  host: clients.aisgroup.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ais Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIS Group, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AIS Group
provider_slug: ais
slug: ais-domain-security
source_filename: ais-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aisgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 02:02:16 2026 GMT\n  hsts: false\n- host: clients.aisgroup.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 19:14:09 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: aisgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ais/refs/heads/main/security/ais-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Finance
- Insurance
- Investment Analytics
- Risk Management
---
