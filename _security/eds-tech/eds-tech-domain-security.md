---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eds.tech
  spf: true
hosts:
- cert_expires: Nov 15 13:32:41 2026 GMT
  host: www.eds.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Energy Design Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Energy Design Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Energy Design Systems
provider_slug: eds-tech
slug: eds-tech-domain-security
source_filename: eds-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eds.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 13:32:41 2026 GMT\n  hsts: false\ndomains:\n- domain: eds.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/eds-tech/security/eds-tech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- HVAC Software
- Load Calculation
- Lead Generation
- Menu Pricing
---
