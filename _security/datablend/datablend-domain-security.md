---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: datablend.com
  spf: true
hosts:
- cert_expires: Dec 29 23:19:03 2026 GMT
  host: datablend.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Datablend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eOne Solutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: eOne Solutions
provider_slug: datablend
slug: datablend-domain-security
source_filename: datablend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datablend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:19:03 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\ndomains:\n- domain: datablend.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/datablend/security/datablend-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- iPaaS
- Data Integration
- Data Virtualization
- Data Migration
- Enterprise
- SaaS
---
