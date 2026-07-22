---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: branchtrack.com
  spf: true
hosts:
- cert_expires: Sep 25 10:33:47 2026 GMT
  host: branchtrack.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Branchtrack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Branchtrack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Branchtrack
provider_slug: branchtrack
slug: branchtrack-domain-security
source_filename: branchtrack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: branchtrack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 10:33:47 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: branchtrack.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/branchtrack/refs/heads/main/security/branchtrack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- E-Learning
- Learning and Development
- Instructional Design
- Simulations
- Branching Scenarios
- SCORM
- xAPI
- Training
---
