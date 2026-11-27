---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: fxlayerhq.com
  spf: true
hosts:
- cert_expires: Jan 23 11:11:25 2027 GMT
  host: fxlayerhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FxLayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FxLayer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: FxLayer
provider_slug: fxlayerhq-com
slug: fxlayerhq-com-domain-security
source_filename: fxlayerhq-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fxlayerhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 11:11:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fxlayerhq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fxlayerhq-com/security/fxlayerhq-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Finance
- Compliance
- Trade
- Export
- Import
---
