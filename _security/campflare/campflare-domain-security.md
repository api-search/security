---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: campflare.com
  spf: false
hosts:
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: campflare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Campflare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Campflare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Campflare
provider_slug: campflare
slug: campflare-domain-security
source_filename: campflare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: campflare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: campflare.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/campflare/refs/heads/main/security/campflare-domain-security.yml
summary_line: TLSv1.3
tags:
- Campgrounds
- Outdoor
- Recreation
- Availability
- Alerts
- Webhooks
- Reservations
---
