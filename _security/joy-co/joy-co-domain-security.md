---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: joy.co
  spf: true
hosts:
- cert_expires: Dec  3 07:47:31 2026 GMT
  host: joy.co
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Joy Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Joy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Joy
provider_slug: joy-co
slug: joy-co-domain-security
source_filename: joy-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joy.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 07:47:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: joy.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/joy-co/security/joy-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Parenting
- Expert Advice
- Tracker
- Telehealth
- Family Support
---
