---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: americanaerospace.com
  spf: true
hosts:
- cert_expires: Oct  8 15:55:51 2026 GMT
  host: americanaerospace.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: American Aerospace Advisors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for American Aerospace Advisors, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: American Aerospace Advisors
provider_slug: american-aerospace-advisors
slug: american-aerospace-advisors-domain-security
source_filename: american-aerospace-advisors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: americanaerospace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 15:55:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: americanaerospace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-aerospace-advisors/refs/heads/main/security/american-aerospace-advisors-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Aerospace
- Defense
- Unmanned Aircraft Systems
- Drones
- Infrastructure Monitoring
- Geospatial
- Sensors
---
