---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ait.ac.at
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.ait.ac.at
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ait Austrian Institute Of Technology Gmbh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIT Austrian Institute of Technology GmbH, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AIT Austrian Institute of Technology GmbH
provider_slug: ait-austrian-institute-of-technology-gmbh
slug: ait-austrian-institute-of-technology-gmbh-domain-security
source_filename: ait-austrian-institute-of-technology-gmbh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ait.ac.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: ait.ac.at\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ait-austrian-institute-of-technology-gmbh/security/ait-austrian-institute-of-technology-gmbh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Research
- Technology
- Infrastructure
- AI
- Energy
---
