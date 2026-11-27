---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: elfy.life
  spf: true
hosts:
- cert_expires: Jan 25 19:19:37 2027 GMT
  host: elfy.life
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Elfy Life Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elfy Life, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Elfy Life
provider_slug: elfy-life
slug: elfy-life-domain-security
source_filename: elfy-life-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elfy.life\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 19:19:37 2027 GMT\n  hsts: false\ndomains:\n- domain: elfy.life\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/elfy-life/security/elfy-life-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Health
- Calculator
- Metabolism
- Nutrition
- French
---
