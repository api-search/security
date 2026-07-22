---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: laserhub.com
  spf: true
hosts:
- cert_expires: Sep 22 19:30:25 2026 GMT
  host: laserhub.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Laserhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laserhub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Laserhub
provider_slug: laserhub
slug: laserhub-domain-security
source_filename: laserhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: laserhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 19:30:25 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: laserhub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laserhub/refs/heads/main/security/laserhub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Manufacturing
- Metal Fabrication
- Procurement
- Laser Cutting
- CNC Machining
- Sheet Metal
- Supply Chain
- Marketplace
- Industrial
- Germany
---
