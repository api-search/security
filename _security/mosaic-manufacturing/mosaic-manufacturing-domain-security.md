---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mosaicmfg.com
  spf: true
hosts:
- cert_expires: Aug 29 17:58:39 2026 GMT
  host: mosaicmfg.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mosaic Manufacturing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mosaic Manufacturing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mosaic Manufacturing
provider_slug: mosaic-manufacturing
slug: mosaic-manufacturing-domain-security
source_filename: mosaic-manufacturing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mosaicmfg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 17:58:39 2026 GMT\n  hsts: false\ndomains:\n- domain: mosaicmfg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mosaic-manufacturing/refs/heads/main/security/mosaic-manufacturing-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- 3D Printing
- Additive Manufacturing
- Manufacturing
- Hardware
- Software
- Robotics
---
