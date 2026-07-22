---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: formenergy.com
  spf: true
hosts:
- cert_expires: Oct  4 13:35:03 2026 GMT
  host: formenergy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Form Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Form Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Form Energy
provider_slug: form-energy
slug: form-energy-domain-security
source_filename: form-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: formenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 13:35:03 2026 GMT\n  hsts: false\ndomains:\n- domain: formenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/form-energy/refs/heads/main/security/form-energy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy Storage
- Long Duration Energy Storage
- Iron-Air Battery
- Battery Storage
- Grid Reliability
- Renewable Energy
- Utility Scale
- Multi-Day Storage
- Grid Modeling
- Clean Energy
- Manufacturing
- West Virginia
---
