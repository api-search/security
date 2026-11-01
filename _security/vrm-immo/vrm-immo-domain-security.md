---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vrm-immo.de
  spf: true
hosts:
- cert_expires: Jan 22 03:44:51 2027 GMT
  host: vrm-immo.de
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vrm Immo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VRM Immo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VRM Immo
provider_slug: vrm-immo
slug: vrm-immo-domain-security
source_filename: vrm-immo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vrm-immo.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 03:44:51 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: vrm-immo.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/vrm-immo/security/vrm-immo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Marketplace
- Germany
- Rhein-Main
---
