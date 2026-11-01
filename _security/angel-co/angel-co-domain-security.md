---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: angel.co
  spf: true
hosts:
- cert_expires: Dec 30 15:39:29 2026 GMT
  host: angel.co
  hsts: true
  hsts_max_age: 631139040
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Angel Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AngelList, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AngelList
provider_slug: angel-co
slug: angel-co-domain-security
source_filename: angel-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: angel.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 15:39:29 2026 GMT\n  hsts: true\n  hsts_max_age: 631139040\ndomains:\n- domain: angel.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/angel-co/security/angel-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Startup
- Recruiting
- JobBoard
- VentureCapital
- Platform
---
