---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mtdt.io
  spf: true
hosts:
- cert_expires: Feb  9 08:18:04 2027 GMT
  host: mtdt.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: mtdt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mtdt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: mtdt
provider_slug: mtdt-io
slug: mtdt-io-domain-security
source_filename: mtdt-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mtdt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 08:18:04 2027 GMT\n  hsts: false\ndomains:\n- domain: mtdt.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mtdt-io/security/mtdt-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Salesforce DevOps
- Deployment
- Backups
- Migrations
- Metadata Management
- Version Control
- Code Analysis
- Release Management
---
