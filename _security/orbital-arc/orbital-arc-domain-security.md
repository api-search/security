---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: orbitalarc.com
  spf: true
hosts:
- cert_expires: Oct  7 23:38:49 2026 GMT
  host: orbitalarc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orbital Arc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orbital Arc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Orbital Arc
provider_slug: orbital-arc
slug: orbital-arc-domain-security
source_filename: orbital-arc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orbitalarc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:38:49 2026 GMT\n  hsts: false\ndomains:\n- domain: orbitalarc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orbital-arc/refs/heads/main/security/orbital-arc-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Space
- Aerospace
- Electric Propulsion
- Satellites
- Deep Tech
- Hardware
---
