---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: skydda.ai
  spf: true
hosts:
- cert_expires: Jan 17 13:43:34 2027 GMT
  host: skydda.ai
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Skydda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skydda, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Skydda
provider_slug: skydda
slug: skydda-domain-security
source_filename: skydda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skydda.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 13:43:34 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: skydda.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/skydda/security/skydda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- AI
- Threat Intelligence
- Defense Platform
---
