---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jobsai.cz
  spf: true
hosts:
- cert_expires: Dec 24 16:31:18 2026 GMT
  host: jobsai.cz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Saleryon s.r.o. Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saleryon s.r.o., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Saleryon s.r.o.
provider_slug: jobsai-cz
slug: jobsai-cz-domain-security
source_filename: jobsai-cz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jobsai.cz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 16:31:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: jobsai.cz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/jobsai-cz/security/jobsai-cz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Job Search
- Czech
- Recruiting
- Platform
---
