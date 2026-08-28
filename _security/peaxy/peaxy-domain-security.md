---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: peaxy.net
  spf: true
hosts:
- cert_expires: Nov 21 02:52:23 2026 GMT
  host: peaxy.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peaxy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peaxy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Peaxy
provider_slug: peaxy
slug: peaxy-domain-security
source_filename: peaxy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: peaxy.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 02:52:23 2026 GMT\n  hsts: false\ndomains:\n- domain: peaxy.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peaxy/refs/heads/main/security/peaxy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Industrial AI
- Digital Twin
- Battery Analytics
- Energy Storage
- Predictive Maintenance
- Asset Management
- Manufacturing
- Defense
- Analytics
- Data Management
- Machine Learning
---
