---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: scaleflux.com
  spf: true
hosts:
- cert_expires: Oct  4 06:18:37 2026 GMT
  host: scaleflux.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scaleflux Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ScaleFlux, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ScaleFlux
provider_slug: scaleflux
slug: scaleflux-domain-security
source_filename: scaleflux-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scaleflux.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 06:18:37 2026 GMT\n  hsts: null\ndomains:\n- domain: scaleflux.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scaleflux/refs/heads/main/security/scaleflux-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Storage
- Hardware
- Semiconductors
- Computational Storage
- NVMe
- SSD
- CXL
- Data Center
- Infrastructure
---
