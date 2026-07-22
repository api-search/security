---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: heliorec.com
  spf: false
hosts:
- cert_expires: Oct  5 18:18:23 2026 GMT
  host: heliorec.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Heliorec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HelioRec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: HelioRec
provider_slug: heliorec
slug: heliorec-domain-security
source_filename: heliorec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heliorec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 18:18:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: heliorec.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heliorec/refs/heads/main/security/heliorec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Floating Solar
- Photovoltaic
- Renewable Energy
- Clean Energy
- Solar Power
- Energy Infrastructure
- Cleantech
---
