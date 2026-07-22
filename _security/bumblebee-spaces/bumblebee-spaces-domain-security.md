---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bumblebeespaces.com
  spf: true
hosts:
- cert_expires: Aug 21 09:02:22 2026 GMT
  host: www.bumblebeespaces.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bumblebee Spaces Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bumblebee Spaces, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bumblebee Spaces
provider_slug: bumblebee-spaces
slug: bumblebee-spaces-domain-security
source_filename: bumblebee-spaces-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bumblebeespaces.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 09:02:22 2026 GMT\n  hsts: false\ndomains:\n- domain: bumblebeespaces.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bumblebee-spaces/refs/heads/main/security/bumblebee-spaces-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Smart Home
- Robotics
- Storage
- Home Automation
- Consumer Hardware
- IoT
- Mobile App
---
