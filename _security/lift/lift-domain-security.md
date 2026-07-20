---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: liftaircraft.com
  spf: true
hosts:
- cert_expires: Oct 13 21:30:13 2026 GMT
  host: www.liftaircraft.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LIFT Aircraft, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LIFT Aircraft
provider_slug: lift
slug: lift-domain-security
source_filename: lift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.liftaircraft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 21:30:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: liftaircraft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lift/refs/heads/main/security/lift-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Aviation
- eVTOL
- Electric Aircraft
- Urban Air Mobility
- Aerospace
- Transportation
- Experiential Entertainment
- Booking
- Model Context Protocol
---
