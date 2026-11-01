---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zynk.com
  spf: true
hosts:
- cert_expires: Jan 14 12:08:48 2027 GMT
  host: zynk.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zynk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zynk Software Limited, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zynk Software Limited
provider_slug: zynk
slug: zynk-domain-security
source_filename: zynk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zynk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 12:08:48 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: zynk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/zynk/security/zynk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Integration
- Automation
- Software-as-a-Service
- Enterprise
---
