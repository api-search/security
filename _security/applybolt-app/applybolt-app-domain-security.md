---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: applybolt.app
  spf: true
hosts:
- cert_expires: Jan  1 19:32:05 2027 GMT
  host: applybolt.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ApplyBolt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ApplyBolt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ApplyBolt
provider_slug: applybolt-app
slug: applybolt-app-domain-security
source_filename: applybolt-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: applybolt.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 19:32:05 2027 GMT\n  hsts: false\ndomains:\n- domain: applybolt.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/applybolt-app/security/applybolt-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Job Search
- ResumeAutomation
- Careers
- Hiring
---
