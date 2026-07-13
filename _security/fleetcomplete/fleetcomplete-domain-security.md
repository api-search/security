---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fleetcomplete.com
  spf: true
hosts:
- cert_expires: Aug 28 12:24:24 2026 GMT
  host: www.fleetcomplete.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 12:03:37 2026 GMT
  host: api.fleetcomplete.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 12:03:37 2026 GMT
  host: tlshosted.fleetcomplete.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fleetcomplete Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fleet Complete, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fleet Complete
provider_slug: fleetcomplete
slug: fleetcomplete-domain-security
source_filename: fleetcomplete-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fleetcomplete.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 12:24:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.fleetcomplete.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 12:03:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tlshosted.fleetcomplete.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 12:03:37 2026 GMT\n  hsts: null\ndomains:\n- domain: fleetcomplete.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fleetcomplete/refs/heads/main/security/fleetcomplete-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fleet Management
- Telematics
- GPS Tracking
- IoT
- GraphQL
- Vehicle Tracking
- Driver Safety
- Geofencing
---
