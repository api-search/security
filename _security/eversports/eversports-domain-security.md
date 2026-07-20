---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: eversports.com
  spf: true
hosts:
- cert_expires: Oct 16 04:53:44 2026 GMT
  host: www.eversports.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eversports Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eversports, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Eversports
provider_slug: eversports
slug: eversports-domain-security
source_filename: eversports-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eversports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 04:53:44 2026 GMT\n  hsts: false\ndomains:\n- domain: eversports.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eversports/refs/heads/main/security/eversports-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Sports
- Fitness
- Booking
- Scheduling
- Wellness
- GraphQL
- Reservations
- Events
---
