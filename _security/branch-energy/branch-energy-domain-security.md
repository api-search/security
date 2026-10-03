---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: branchenergy.com
  spf: true
hosts:
- cert_expires: Dec 14 22:15:10 2026 GMT
  host: branchenergy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Branch Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Branch Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Branch Energy
provider_slug: branch-energy
slug: branch-energy-domain-security
source_filename: branch-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: branchenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 22:15:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: branchenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/branch-energy/refs/heads/main/security/branch-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Electricity
- BatteryStorage
- Texas
- Retail
---
