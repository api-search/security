---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: caiso.com
  spf: true
hosts:
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: www.caiso.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: oasis.caiso.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Caiso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for California ISO, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: California ISO
provider_slug: caiso
slug: caiso-domain-security
source_filename: caiso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caiso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: false\n- host: oasis.caiso.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: caiso.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caiso/refs/heads/main/security/caiso-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- United States
- Electricity
- Energy Markets
- Grid
- Renewables
- System Operator
- Market Data
- California
---
