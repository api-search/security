---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: convradar.com
  spf: true
hosts:
- cert_expires: Jan  5 13:22:59 2027 GMT
  host: convradar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Conversion Radar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conversion Radar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Conversion Radar
provider_slug: convradar-com
slug: convradar-com-domain-security
source_filename: convradar-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: convradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 13:22:59 2027 GMT\n  hsts: false\ndomains:\n- domain: convradar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/convradar-com/security/convradar-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Analytics
- Google Analytics 4
- MCP
- Conversion Rate Optimization
- E-Commerce
- Benchmarks
- AI Agents
---
