---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datacor.com
  spf: true
hosts:
- cert_expires: Sep 26 18:13:00 2026 GMT
  host: datacor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datacor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datacor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Datacor
provider_slug: datacor
slug: datacor-domain-security
source_filename: datacor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datacor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 18:13:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: datacor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datacor/refs/heads/main/security/datacor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Software
- ERP
- Process Manufacturing
- Chemical Distribution
- Chemical Process Simulation
- Formulation Management
- LIMS
- Animal Nutrition
- Manufacturing
---
