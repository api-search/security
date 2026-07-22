---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rexby.com
  spf: true
hosts:
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: rexby.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rexby Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rexby, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rexby
provider_slug: rexby
slug: rexby-domain-security
source_filename: rexby-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rexby.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: rexby.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rexby/refs/heads/main/security/rexby-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel
- Travel Guides
- Maps
- Trip Planning
- Creator Economy
- Consumer App
- Mobile
---
