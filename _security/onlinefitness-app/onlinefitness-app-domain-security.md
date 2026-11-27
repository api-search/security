---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: onlinefitness.app
  spf: false
hosts:
- cert_expires: Jan 13 08:12:56 2027 GMT
  host: onlinefitness.app
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Online Fitness Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Online Fitness, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=quarantine).'
provider_name: Online Fitness
provider_slug: onlinefitness-app
slug: onlinefitness-app-domain-security
source_filename: onlinefitness-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onlinefitness.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 08:12:56 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: onlinefitness.app\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/onlinefitness-app/security/onlinefitness-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fitness
- Coaching
- Software-as-a-Service
- Health Tech
- Personal Training
---
