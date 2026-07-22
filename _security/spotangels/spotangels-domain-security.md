---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: spotangels.com
  spf: true
hosts:
- cert_expires: Sep 21 21:59:46 2026 GMT
  host: www.spotangels.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spotangels Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spotangels, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Spotangels
provider_slug: spotangels
slug: spotangels-domain-security
source_filename: spotangels-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spotangels.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 21:59:46 2026 GMT\n  hsts: false\ndomains:\n- domain: spotangels.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spotangels/refs/heads/main/security/spotangels-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Parking
- Mobility
- Transportation
- Consumer App
- Location
- Y Combinator
---
