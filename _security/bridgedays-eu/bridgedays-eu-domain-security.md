---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bridgedays.eu
  spf: true
hosts:
- cert_expires: Dec  9 03:41:53 2026 GMT
  host: bridgedays.eu
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BridgeDays Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BridgeDays, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BridgeDays
provider_slug: bridgedays-eu
slug: bridgedays-eu-domain-security
source_filename: bridgedays-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bridgedays.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 03:41:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bridgedays.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bridgedays-eu/security/bridgedays-eu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Planner
- Holidays
- Vacation
- Free
---
