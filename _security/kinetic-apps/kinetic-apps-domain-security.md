---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kineticapps.ai
  spf: true
hosts:
- cert_expires: Oct  4 02:19:08 2026 GMT
  host: www.kineticapps.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kinetic Apps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kinetic Apps, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kinetic Apps
provider_slug: kinetic-apps
slug: kinetic-apps-domain-security
source_filename: kinetic-apps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kineticapps.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 02:19:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kineticapps.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kinetic-apps/refs/heads/main/security/kinetic-apps-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- Venture Studio
- Consumer Software
- Startup Studio
- App Portfolio
- Product Development
---
