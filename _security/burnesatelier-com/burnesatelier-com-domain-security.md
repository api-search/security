---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: burnesatelier.com
  spf: false
hosts:
- cert_expires: Jan 31 00:34:45 2027 GMT
  host: burnesatelier.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Burnesatelier Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Burnes Atelier, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Burnes Atelier
provider_slug: burnesatelier-com
slug: burnesatelier-com-domain-security
source_filename: burnesatelier-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: burnesatelier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 00:34:45 2027 GMT\n  hsts: false\ndomains:\n- domain: burnesatelier.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/burnesatelier-com/security/burnesatelier-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Business
- Automation
- Integration
- Monitoring
- Risk Management
---
