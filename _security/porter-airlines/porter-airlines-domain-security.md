---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flyporter.com
  spf: true
hosts:
- cert_expires: Aug 23 06:22:41 2026 GMT
  host: www.flyporter.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Porter Airlines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Porter Airlines, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Porter Airlines
provider_slug: porter-airlines
slug: porter-airlines-domain-security
source_filename: porter-airlines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flyporter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 06:22:41 2026 GMT\n  hsts: null\ndomains:\n- domain: flyporter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/porter-airlines/refs/heads/main/security/porter-airlines-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- Canada
- Aviation
- Airline
- Flights
- Distribution
- GDS
- Booking
- Travel Agents
- Loyalty
---
