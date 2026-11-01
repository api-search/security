---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lemni.com
  spf: false
hosts:
- cert_expires: Jan  4 03:22:40 2027 GMT
  host: www.lemni.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lemni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lemni, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Lemni
provider_slug: lemni
slug: lemni-domain-security
source_filename: lemni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lemni.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 03:22:40 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lemni.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/lemni/security/lemni-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI
- Customer-Engagement
- SaaS
- Automation
- Platform
---
