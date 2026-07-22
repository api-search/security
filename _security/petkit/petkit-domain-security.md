---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: petkit.com
  spf: true
hosts:
- cert_expires: Aug 27 23:31:01 2026 GMT
  host: petkit.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Petkit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for petkit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: petkit
provider_slug: petkit
slug: petkit-domain-security
source_filename: petkit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: petkit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 23:31:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: petkit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/petkit/refs/heads/main/security/petkit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Pet Tech
- Smart Home
- Internet of Things
- Consumer Electronics
- E-Commerce
---
