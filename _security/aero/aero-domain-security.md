---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aero.com
  spf: true
hosts:
- cert_expires: Oct  1 03:22:53 2026 GMT
  host: aero.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aero
provider_slug: aero
slug: aero-domain-security
source_filename: aero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:22:53 2026 GMT\n  hsts: false\ndomains:\n- domain: aero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aero/refs/heads/main/security/aero-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel
- Air Travel
- Airlines
- Private Aviation
- Transportation
- Booking
- Consumer
---
