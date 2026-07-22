---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: setscouter.com
  spf: true
hosts:
- cert_expires: Oct 18 20:58:34 2026 GMT
  host: setscouter.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Set Scouter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Set Scouter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Set Scouter
provider_slug: set-scouter
slug: set-scouter-domain-security
source_filename: set-scouter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: setscouter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 20:58:34 2026 GMT\n  hsts: false\ndomains:\n- domain: setscouter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/set-scouter/refs/heads/main/security/set-scouter-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Location Scouting
- Film Production
- Marketplace
- Media and Entertainment
- Booking
- Real Estate
---
