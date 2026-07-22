---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nov.com
  spf: true
hosts:
- cert_expires: Sep 11 21:24:51 2026 GMT
  host: www.nov.com
  hsts: true
  hsts_max_age: 18410000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Oilwell Varco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Oilwell Varco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: National Oilwell Varco
provider_slug: national-oilwell-varco
slug: national-oilwell-varco-domain-security
source_filename: national-oilwell-varco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nov.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 21:24:51 2026 GMT\n  hsts: true\n  hsts_max_age: 18410000\ndomains:\n- domain: nov.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-oilwell-varco/refs/heads/main/security/national-oilwell-varco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Oil and Gas
- Drilling
- Energy
- Industrial
- Fortune 500
---
