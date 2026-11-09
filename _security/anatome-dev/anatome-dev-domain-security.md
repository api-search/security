---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: anatome.dev
  spf: true
hosts:
- cert_expires: Jan  7 13:21:10 2027 GMT
  host: anatome.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anatome Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anatome, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Anatome
provider_slug: anatome-dev
slug: anatome-dev-domain-security
source_filename: anatome-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anatome.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 13:21:10 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: anatome.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/anatome-dev/security/anatome-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Fitness
- Nutrition
- Artificial Intelligence
- Health
- Workout Tracking
---
