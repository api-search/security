---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aim-journal.com
  spf: false
hosts:
- cert_expires: Dec  3 23:42:44 2026 GMT
  host: aim-journal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AIm Workout Journal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIm Workout Journal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: AIm Workout Journal
provider_slug: aim-journal-com
slug: aim-journal-com-domain-security
source_filename: aim-journal-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aim-journal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:42:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aim-journal.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aim-journal-com/security/aim-journal-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fitness
- Artificial Intelligence
- Workouts
- Health
- Personalization
---
