---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ford.com
  spf: true
hosts:
- cert_expires: Sep 21 10:48:50 2026 GMT
  host: www.ford.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.ford.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- cert_expires: Sep  8 04:15:49 2026 GMT
  host: developerportal.ford.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fordpass Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FordPass / Ford Pro, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FordPass / Ford Pro
provider_slug: fordpass
slug: fordpass-domain-security
source_filename: fordpass-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ford.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 10:48:50 2026 GMT\n  hsts: null\n- host: developer.ford.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: developerportal.ford.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 04:15:49 2026 GMT\n  hsts: false\ndomains:\n- domain: ford.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fordpass/refs/heads/main/security/fordpass-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automotive
- Connected Vehicle
- Connected Car
- Telematics
- Fleet
- Fleet Management
- Vehicle Data
- Vehicle Health
- Remote Commands
- OEM
- Mobility
- FordPass
- Ford Pro
- FordConnect
- BlueCruise
- Electric Vehicles
- EV Charging
- Phone As A Key
- SYNC
---
