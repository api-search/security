---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: comfortsystemsusa.com
  spf: true
hosts:
- cert_expires: Aug 23 01:53:57 2026 GMT
  host: www.comfortsystemsusa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.comfortsystemsusa.com
  https: false
- host: api.comfortsystemsusa.com
  https: false
kind: domain-security
layout: security
method: probed
name: Comfort Systems Usa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Comfort Systems USA, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Comfort Systems USA
provider_slug: comfort-systems-usa
slug: comfort-systems-usa-domain-security
source_filename: comfort-systems-usa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.comfortsystemsusa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 01:53:57 2026 GMT\n  hsts: false\n- host: developer.comfortsystemsusa.com\n  https: false\n- host: api.comfortsystemsusa.com\n  https: false\ndomains:\n- domain: comfortsystemsusa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comfort-systems-usa/refs/heads/main/security/comfort-systems-usa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- HVAC
- Mechanical
- Construction
---
