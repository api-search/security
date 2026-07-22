---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: explomar.tech
  spf: false
hosts:
- cert_expires: Sep 15 08:14:44 2026 GMT
  host: www.explomar.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Explomar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Explomar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Explomar
provider_slug: explomar
slug: explomar-domain-security
source_filename: explomar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.explomar.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 08:14:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: explomar.tech\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/explomar/refs/heads/main/security/explomar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Marine
- Electric Propulsion
- Outboard Motors
- Marine Hardware
- Clean Energy
- Boating
- Electric Vehicles
---
