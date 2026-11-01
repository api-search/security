---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: moneta.health
  spf: true
hosts:
- cert_expires: Dec 24 14:15:13 2026 GMT
  host: moneta.health
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Moneta Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moneta Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Moneta Health
provider_slug: moneta-health
slug: moneta-health-domain-security
source_filename: moneta-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moneta.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 14:15:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: moneta.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/moneta-health/security/moneta-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Memory
- Telehealth
- Cognitive Rehabilitation
- At-Home Care
---
