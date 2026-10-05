---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: boxpower.io
  spf: true
hosts:
- cert_expires: Nov 29 15:59:26 2026 GMT
  host: boxpower.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Boxpower Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boxpower, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Boxpower
provider_slug: boxpower
slug: boxpower-domain-security
source_filename: boxpower-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boxpower.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 15:59:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: boxpower.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boxpower/refs/heads/main/security/boxpower-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Microgrid
- Renewables
- Infrastructure
---
