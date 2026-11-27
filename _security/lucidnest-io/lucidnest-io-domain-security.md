---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: lucidnest.io
  spf: true
hosts:
- cert_expires: Feb  3 09:16:12 2027 GMT
  host: lucidnest.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LucidNest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LucidNest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: LucidNest
provider_slug: lucidnest-io
slug: lucidnest-io-domain-security
source_filename: lucidnest-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lucidnest.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 09:16:12 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: lucidnest.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lucidnest-io/security/lucidnest-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Productivity
- Note Taking
- Task Management
- Artificial Intelligence
- Quebec
---
