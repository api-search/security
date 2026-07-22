---
description: ''
domains:
- caa:
  - 0 iodef "mailto:dev@thedyrt.com"
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: thedyrt.com
  spf: true
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: thedyrt.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dyrt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dyrt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Dyrt
provider_slug: dyrt
slug: dyrt-domain-security
source_filename: dyrt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thedyrt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: thedyrt.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:dev@thedyrt.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dyrt/refs/heads/main/security/dyrt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Camping
- Campgrounds
- RV
- Travel
- Outdoor Recreation
- Reviews
- Booking
- Consumer App
---
