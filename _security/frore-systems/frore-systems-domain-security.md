---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: froresystems.com
  spf: true
hosts:
- cert_expires: Sep 11 18:01:57 2026 GMT
  host: froresystems.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Frore Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frore Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Frore Systems
provider_slug: frore-systems
slug: frore-systems-domain-security
source_filename: frore-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: froresystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 18:01:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: froresystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frore-systems/refs/heads/main/security/frore-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Thermal Management
- Semiconductors
- Hardware
- Cooling
- Data Center
- Solid State Cooling
---
