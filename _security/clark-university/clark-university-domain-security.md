---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clarku.edu
  spf: true
hosts:
- cert_expires: Dec 24 21:47:34 2026 GMT
  host: www.clarku.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clark University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clark University, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clark University
provider_slug: clark-university
slug: clark-university-domain-security
source_filename: clark-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clarku.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 21:47:34 2026 GMT\n  hsts: false\ndomains:\n- domain: clarku.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/clark-university/security/clark-university-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- University
- Research
- Worcester
- HigherEd
- Company
---
