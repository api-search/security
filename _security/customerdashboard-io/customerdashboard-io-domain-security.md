---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: customerdashboard.io
  spf: true
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: customerdashboard.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CustomerDashboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CustomerDashboard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CustomerDashboard
provider_slug: customerdashboard-io
slug: customerdashboard-io-domain-security
source_filename: customerdashboard-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: customerdashboard.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: customerdashboard.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/customerdashboard-io/security/customerdashboard-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Analytics
- Dashboards
- Customer-Facing Analytics
- Embedded Analytics
- Client Reporting
- White Label
- Multi-Tenant
- MCP
- Software-as-a-Service
---
