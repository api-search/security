---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: appie.run
  spf: true
hosts:
- cert_expires: Dec  8 04:07:40 2026 GMT
  host: appie.run
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Appie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Appie
provider_slug: appie-run
slug: appie-run-domain-security
source_filename: appie-run-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appie.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 04:07:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: appie.run\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/appie-run/security/appie-run-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Marketing
- Automation
- Software-as-a-Service
- Platform
---
