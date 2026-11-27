---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iknowthepilot.com.au
  spf: true
hosts:
- cert_expires: Dec 30 13:54:34 2026 GMT
  host: iknowthepilot.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: I Know The Pilot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for I Know The Pilot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: I Know The Pilot
provider_slug: iknowthepilot-com-au
slug: iknowthepilot-com-au-domain-security
source_filename: iknowthepilot-com-au-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iknowthepilot.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 13:54:34 2026 GMT\n  hsts: null\ndomains:\n- domain: iknowthepilot.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/iknowthepilot-com-au/security/iknowthepilot-com-au-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- Flights
- Deals
- Australia
- Aggregator
---
