---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: xentity.com
  spf: true
hosts:
- cert_expires: Dec 22 06:36:41 2026 GMT
  host: www.xentity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Xentity Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xentity Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Xentity Corporation
provider_slug: xentity-corporation
slug: xentity-corporation-domain-security
source_filename: xentity-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xentity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 06:36:41 2026 GMT\n  hsts: false\ndomains:\n- domain: xentity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/xentity-corporation/security/xentity-corporation-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- IT Consulting
- Data Integration
- Big Data
- IoT
---
