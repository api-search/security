---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ecoplanet.tech
  spf: true
hosts:
- cert_expires: Sep 29 22:36:46 2026 GMT
  host: www.ecoplanet.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ecoplanet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ecoplanet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ecoplanet
provider_slug: ecoplanet
slug: ecoplanet-domain-security
source_filename: ecoplanet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ecoplanet.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 22:36:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ecoplanet.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecoplanet/refs/heads/main/security/ecoplanet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Climate
- Energy
- Energy Management
- Sustainability
- ISO 50001
- Energy Procurement
- Software
- Germany
---
