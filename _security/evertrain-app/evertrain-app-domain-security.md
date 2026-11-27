---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: evertrain.app
  spf: true
hosts:
- cert_expires: Jan 25 06:04:39 2027 GMT
  host: evertrain.app
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Evertrain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evertrain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Evertrain
provider_slug: evertrain-app
slug: evertrain-app-domain-security
source_filename: evertrain-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evertrain.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 06:04:39 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: evertrain.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/evertrain-app/security/evertrain-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Fitness
- Health
- Training
---
