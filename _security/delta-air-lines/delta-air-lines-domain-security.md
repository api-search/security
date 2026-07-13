---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: delta.com
  spf: true
hosts:
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: www.delta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: apiportal.delta.com
  https: false
kind: domain-security
layout: security
method: probed
name: Delta Air Lines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Delta Air Lines, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Delta Air Lines
provider_slug: delta-air-lines
slug: delta-air-lines-domain-security
source_filename: delta-air-lines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.delta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: false\n- host: apiportal.delta.com\n  https: false\ndomains:\n- domain: delta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delta-air-lines/refs/heads/main/security/delta-air-lines-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Air Travel
- Airlines
- Aviation
- Booking
- Flights
- NDC
- Travel
- Fortune 100
---
