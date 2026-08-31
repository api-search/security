---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: super.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: snaptravel.com
  spf: true
hosts:
- cert_expires: Oct 16 22:48:48 2026 GMT
  host: www.super.com
  hsts: true
  hsts_header: max-age=2592000; includeSubDomains; preload
  hsts_max_age: 2592000
  https: true
  note: The automated HTTP probe recorded null because every HTML path on www.super.com answers a 403 Cloudflare bot challenge; the header was read directly from a 200 response (https://www.super.com/robots.txt) on 2026-08-05.
  tls_version: TLSv1.3
- cert_expires: Sep  6 18:16:09 2026 GMT
  host: api.snaptravel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Supercom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Super.com, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Super.com
provider_slug: supercom
slug: supercom-domain-security
source_filename: supercom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.super.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 22:48:48 2026 GMT\n  hsts: true\n  hsts_header: max-age=2592000; includeSubDomains; preload\n  hsts_max_age: 2592000\n  note: >-\n    The automated HTTP probe recorded null because every HTML path on www.super.com answers a\n    403 Cloudflare bot challenge; the header was read directly from a 200 response\n    (https://www.super.com/robots.txt) on 2026-08-05.\n- host: api.snaptravel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 18:16:09 2026 GMT\n  hsts: false\ndomains:\n- domain: super.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: snaptravel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supercom/refs/heads/main/security/supercom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Hotels
- Booking
- Flights
- Consumer Finance
- Cash Back
- Savings
- Prescription Discounts
- Mobile Applications
---
