---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: jobily.gr
  spf: true
hosts:
- cert_expires: Dec 27 23:43:17 2026 GMT
  host: jobily.gr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jobily Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jobily, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Jobily
provider_slug: jobily-gr
slug: jobily-gr-domain-security
source_filename: jobily-gr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jobily.gr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:43:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jobily.gr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/jobily-gr/security/jobily-gr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Job
- Recruiting
- Greece
- Careers
- Hiring
---
