---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mdpgroup.com
  spf: true
hosts:
- cert_expires: Dec 23 12:45:28 2026 GMT
  host: mdpgroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mdpgroup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MDP Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MDP Group
provider_slug: mdpgroup
slug: mdpgroup-domain-security
source_filename: mdpgroup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mdpgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 12:45:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mdpgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mdpgroup/security/mdpgroup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SAP Consulting
- Integration
- E-Invoicing
- AI Solutions
- ERP Add‑ons
- Procurement
- Continuous Improvement
---
