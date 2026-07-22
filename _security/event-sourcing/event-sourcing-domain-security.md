---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: martinfowler.com
  spf: false
hosts:
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: martinfowler.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Event Sourcing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Event Sourcing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Event Sourcing
provider_slug: event-sourcing
slug: event-sourcing-domain-security
source_filename: event-sourcing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: martinfowler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: martinfowler.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/event-sourcing/refs/heads/main/security/event-sourcing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Architecture
- CQRS
- Distributed Systems
- Event Sourcing
---
