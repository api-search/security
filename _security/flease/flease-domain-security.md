---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flease.fr
  spf: true
hosts:
- cert_expires: Oct  1 20:15:02 2026 GMT
  host: www.flease.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flease Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flease, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Flease
provider_slug: flease
slug: flease-domain-security
source_filename: flease-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flease.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 20:15:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flease.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flease/refs/heads/main/security/flease-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketplace
- Automotive
- Vehicle Leasing
- Fleet Management
- Mobility
- France
---
