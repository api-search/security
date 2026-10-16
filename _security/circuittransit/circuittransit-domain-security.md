---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ridecircuit.com
  spf: true
hosts:
- cert_expires: Dec 16 06:46:55 2026 GMT
  host: www.ridecircuit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Circuittransit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Circuittransit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Circuittransit
provider_slug: circuittransit
slug: circuittransit-domain-security
source_filename: circuittransit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ridecircuit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 06:46:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ridecircuit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circuittransit/refs/heads/main/security/circuittransit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Transportation
- Electric Vehicles
- On-demand Mobility
- SaaS
---
