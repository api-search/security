---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aviyair.com
  spf: true
hosts:
- cert_expires: Sep 18 20:54:34 2026 GMT
  host: aviyair.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aviyair Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aviyair, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aviyair
provider_slug: aviyair
slug: aviyair-domain-security
source_filename: aviyair-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aviyair.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 20:54:34 2026 GMT\n  hsts: false\ndomains:\n- domain: aviyair.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aviyair/refs/heads/main/security/aviyair-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Airlines
- Airports
- Aviation
- Flight Tracking
- IATA
---
