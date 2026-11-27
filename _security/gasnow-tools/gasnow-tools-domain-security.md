---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gasnow.tools
  spf: true
hosts:
- cert_expires: Jan 10 00:19:28 2027 GMT
  host: gasnow.tools
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GasNow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GasNow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GasNow
provider_slug: gasnow-tools
slug: gasnow-tools-domain-security
source_filename: gasnow-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gasnow.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 00:19:28 2027 GMT\n  hsts: false\ndomains:\n- domain: gasnow.tools\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gasnow-tools/security/gasnow-tools-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cryptocurrency
- Analytics
- GasFees
- Dashboards
- Real-Time
- Free
---
