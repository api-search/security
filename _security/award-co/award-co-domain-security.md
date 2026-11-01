---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: award.co
  spf: false
hosts:
- cert_expires: Dec  2 01:10:03 2026 GMT
  host: www.award.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Award Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Awardco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Awardco
provider_slug: award-co
slug: award-co-domain-security
source_filename: award-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.award.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 01:10:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: award.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/award-co/security/award-co-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- SaaS
- Employee Engagement
- Rewards
- Recognition
---
