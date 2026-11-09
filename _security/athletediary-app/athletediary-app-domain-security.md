---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: athletediary.app
  spf: true
hosts:
- cert_expires: Jan 14 10:42:46 2027 GMT
  host: athletediary.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Athletediary App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Athlete Diary, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Athlete Diary
provider_slug: athletediary-app
slug: athletediary-app-domain-security
source_filename: athletediary-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: athletediary.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 10:42:46 2027 GMT\n  hsts: false\ndomains:\n- domain: athletediary.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/athletediary-app/security/athletediary-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fitness
- Health
- Artificial Intelligence
- Telegram
- iOS
---
