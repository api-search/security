---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: eversports.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: eversportsmanager.com
  spf: true
hosts:
- cert_expires: Oct 16 04:53:44 2026 GMT
  host: www.eversports.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 10:06:34 2026 GMT
  host: helpcenter.eversportsmanager.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 05:10:30 2026 GMT
  host: provider-api.eversportsmanager.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eversport Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eversports, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Eversports
provider_slug: eversport
slug: eversport-domain-security
source_filename: eversport-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eversports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 04:53:44 2026 GMT\n  hsts: false\n- host: helpcenter.eversportsmanager.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 10:06:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: provider-api.eversportsmanager.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 05:10:30 2026 GMT\n  hsts: null\ndomains:\n- domain: eversports.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: eversportsmanager.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eversport/refs/heads/main/security/eversport-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Sports
- Fitness
- Booking
- Scheduling
- Wellness
- Marketplace
- GraphQL
- Reservations
- Studio Management
- Events
---
