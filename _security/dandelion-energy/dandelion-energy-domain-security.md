---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dandelionenergy.com
  spf: true
hosts:
- cert_expires: Sep 25 12:49:16 2026 GMT
  host: dandelionenergy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dandelion Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dandelion Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dandelion Energy
provider_slug: dandelion-energy
slug: dandelion-energy-domain-security
source_filename: dandelion-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dandelionenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 12:49:16 2026 GMT\n  hsts: false\ndomains:\n- domain: dandelionenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dandelion-energy/refs/heads/main/security/dandelion-energy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Geothermal
- Energy
- HVAC
- Heat Pumps
- Climate Tech
- Clean Energy
- Home Services
- Frontier Tech
---
