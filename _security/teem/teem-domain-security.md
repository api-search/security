---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: teem.com
  spf: true
hosts:
- cert_expires: Sep  4 18:10:52 2026 GMT
  host: teem.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Teem
provider_slug: teem
slug: teem-domain-security
source_filename: teem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: teem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 18:10:52 2026 GMT\n  hsts: false\ndomains:\n- domain: teem.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teem/refs/heads/main/security/teem-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Enterprise
- Meeting Rooms
- Workplace
- Scheduling
- Desk Booking
- Visitor Management
- Room Booking
- Space Management
- Facilities
---
