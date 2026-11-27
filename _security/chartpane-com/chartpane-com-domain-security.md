---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: chartpane.com
  spf: true
hosts:
- cert_expires: Jan  2 15:50:14 2027 GMT
  host: chartpane.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ChartPane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChartPane, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: ChartPane
provider_slug: chartpane-com
slug: chartpane-com-domain-security
source_filename: chartpane-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chartpane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 15:50:14 2027 GMT\n  hsts: false\ndomains:\n- domain: chartpane.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/chartpane-com/security/chartpane-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Data Visualization
- AI Integration
- No-Code
- Charts
- Business Intelligence
---
