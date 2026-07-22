---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sunairio.com
  spf: true
hosts:
- cert_expires: Sep 16 00:25:50 2026 GMT
  host: sunairio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sunairio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sunairio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sunairio
provider_slug: sunairio
slug: sunairio-domain-security
source_filename: sunairio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sunairio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 00:25:50 2026 GMT\n  hsts: false\ndomains:\n- domain: sunairio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sunairio/refs/heads/main/security/sunairio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Weather
- Climate
- Forecasting
- Grid
- Data
- Analytics
- Power Markets
---
