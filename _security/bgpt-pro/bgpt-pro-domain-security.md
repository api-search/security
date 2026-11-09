---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bgpt.pro
  spf: true
hosts:
- cert_expires: Jan 21 06:45:17 2027 GMT
  host: bgpt.pro
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bgpt Pro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BGPT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BGPT
provider_slug: bgpt-pro
slug: bgpt-pro-domain-security
source_filename: bgpt-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bgpt.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 06:45:17 2027 GMT\n  hsts: false\ndomains:\n- domain: bgpt.pro\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bgpt-pro/security/bgpt-pro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Scientific
- Evidence
- Research
- Data
---
