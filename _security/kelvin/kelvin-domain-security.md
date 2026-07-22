---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: go-kelvin.com
  spf: true
hosts:
- cert_expires: Sep 11 18:56:14 2026 GMT
  host: go-kelvin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kelvin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kelvin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kelvin
provider_slug: kelvin
slug: kelvin-domain-security
source_filename: kelvin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: go-kelvin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 18:56:14 2026 GMT\n  hsts: null\ndomains:\n- domain: go-kelvin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kelvin/refs/heads/main/security/kelvin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Energy Efficiency
- Home Renovation
- Construction
- Artificial Intelligence
- Lead Generation
- Sales Enablement
- France
- Sustainability
---
