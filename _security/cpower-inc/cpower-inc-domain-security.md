---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cpowerenergy.com
  spf: true
hosts:
- cert_expires: Sep 16 01:24:57 2026 GMT
  host: cpowerenergy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cpower Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CPower, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CPower, Inc.
provider_slug: cpower-inc
slug: cpower-inc-domain-security
source_filename: cpower-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cpowerenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:24:57 2026 GMT\n  hsts: false\ndomains:\n- domain: cpowerenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cpower-inc/refs/heads/main/security/cpower-inc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Deep Tech
- Energy
- Demand Response
- Virtual Power Plant
- Distributed Energy Resources
- Grid Flexibility
- Sustainability
---
