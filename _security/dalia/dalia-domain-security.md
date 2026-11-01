---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dalia.co
  spf: true
hosts:
- cert_expires: Nov 23 14:09:21 2026 GMT
  host: www.dalia.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dalia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dalia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dalia
provider_slug: dalia
slug: dalia-domain-security
source_filename: dalia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dalia.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 14:09:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dalia.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dalia/security/dalia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Recruiting
- Human Resources
- Software-as-a-Service
- CandidateConversion
- Job Board
---
