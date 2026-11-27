---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: currentcost.com
  spf: true
hosts:
- cert_expires: Jan 22 08:40:26 2027 GMT
  host: currentcost.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Current Cost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Current Cost, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Current Cost
provider_slug: current-cost
slug: current-cost-domain-security
source_filename: current-cost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: currentcost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 08:40:26 2027 GMT\n  hsts: false\ndomains:\n- domain: currentcost.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/current-cost/security/current-cost-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- IoT
- Smart Home
- Utilities
---
