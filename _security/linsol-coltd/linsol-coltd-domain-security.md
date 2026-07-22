---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: linsol.kr
  spf: true
hosts:
- cert_expires: Sep 24 09:04:51 2026 GMT
  host: linsol.kr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Linsol Coltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LINSOL Co.,Ltd., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LINSOL Co.,Ltd.
provider_slug: linsol-coltd
slug: linsol-coltd-domain-security
source_filename: linsol-coltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linsol.kr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 09:04:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: linsol.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linsol-coltd/refs/heads/main/security/linsol-coltd-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Safety
- Industrial Safety
- Internet of Things
- Hardware
- Acoustics
- Sensors
- Location Tracking
- Defense
- ESG
- South Korea
---
