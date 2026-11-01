---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: psu.edu
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: www.arl.psu.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Penn State Applied Research Lab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Penn State Applied Research Lab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Penn State Applied Research Lab
provider_slug: penn-state-applied-research-lab
slug: penn-state-applied-research-lab-domain-security
source_filename: penn-state-applied-research-lab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arl.psu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: psu.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/penn-state-applied-research-lab/security/penn-state-applied-research-lab-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Research
- Engineering
- University
- Defense
- Technology
---
