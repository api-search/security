---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: psdcitywide.com
  spf: true
hosts:
- cert_expires: Sep  3 17:46:30 2026 GMT
  host: psdcitywide.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Psdcitywide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PSD Citywide, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PSD Citywide
provider_slug: psdcitywide
slug: psdcitywide-domain-security
source_filename: psdcitywide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: psdcitywide.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 17:46:30 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: psdcitywide.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/psdcitywide/refs/heads/main/security/psdcitywide-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Government
- GovTech
- Asset Management
- Enterprise Asset Management
- Municipal Software
- Public Sector
- SaaS
- GIS
- Permitting
---
