---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vertical.bar
  spf: true
hosts:
- cert_expires: Aug 27 14:10:16 2026 GMT
  host: vertical.bar
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vertical Bar Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vertical Bar Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vertical Bar Inc.
provider_slug: vertical-bar-inc
slug: vertical-bar-inc-domain-security
source_filename: vertical-bar-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vertical.bar\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 14:10:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vertical.bar\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vertical-bar-inc/refs/heads/main/security/vertical-bar-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- NetSuite
- DevOps
- ERP
- Change Management
- Process Mining
- Configuration Management
- Manufacturing
---
