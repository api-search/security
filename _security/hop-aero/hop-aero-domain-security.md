---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hop-aero.com
  spf: true
hosts:
- cert_expires: Oct  8 11:56:24 2026 GMT
  host: hop-aero.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hop Aero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hop Aero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hop Aero
provider_slug: hop-aero
slug: hop-aero-domain-security
source_filename: hop-aero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hop-aero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 11:56:24 2026 GMT\n  hsts: false\ndomains:\n- domain: hop-aero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hop-aero/refs/heads/main/security/hop-aero-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Aerospace
- Defense
- Space
- Logistics
- Rocketry
- Hypersonics
- Y Combinator
---
